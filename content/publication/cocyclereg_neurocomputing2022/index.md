---
title: 'CoCycleReg: Collaborative Cycle-consistency Method for Multi-modal Medical Image Registration. Neurocomputing'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Xiaomeng Li
  - Lingke Kong
  - Jiacheng Wang
  - Wei Zhang
  - Xiaoyang Huang
  - Liansheng Wang

# Author notes (optional)
author_notes:
  # - 'Equal contribution'
  # - 'Equal contribution'

# Schedule page publish date (NOT publication's date).
publishDate: '2022-08-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
# publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *Neurocomputing*
publication_short: In *Neurocomputing*


# abstract: Supervised Pix2Pix and unsupervised Cycle-consistency are two modes that dominate the field of medical image-to-image translation. However, neither modes are ideal. The Pix2Pix mode has excellent performance. But it requires paired and well pixel-wise aligned images, which may not always be achievable due to respiratory motion or anatomy change between times that paired images are acquired. The Cycle-consistency mode is less stringent with training data and works well on unpaired or misaligned images. But its performance may not be optimal. In order to break the dilemma of the existing modes, we propose a new unsupervised mode called RegGAN for medical image-to-image translation. It is based on the theory of "loss-correction". In RegGAN, the misaligned target images are considered as noisy labelsaand the generator is trained with an additional registration network to fit the misaligned noise distribution adaptively.The goal is to search for the common optimal solution to both image-to-image translation and registration tasks. We incorporated RegGAN into a few state-of-the-art image-to-image translation methods and demonstrated that RegGAN could be easily combined with these methods to improve their performances. Such as a simple CycleGAN in our mode surpasses latest NICEGAN even though using less network parameters. Based on our results, RegGAN outperformed both Pix2Pix on aligned data and Cycle-consistency on misaligned or unpaired data. RegGAN is insensitive to noises which makes it a better choice for a wide range of scenarios, especially for medical image-to-image translation tasks in which well pixel-wise aligned data are not available. Code and data used in this study can be found at https://github.com/Kid-Liet/Reg-GAN.


# Summary. An optional shortened abstract.
summary: Collaborative registration-translation cycle-consistency.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://www.sciencedirect.com/science/article/abs/pii/S0925231222006993'
url_code: 'https://github.com/DopamineLcy/cocycle-reg/'
# url_dataset: 'https://github.com/wowchemy/wowchemy-hugo-themes'
# url_poster: ''
# url_project: ''
# url_slides: ''
# url_source: 'https://github.com/wowchemy/wowchemy-hugo-themes'
# url_video: 'https://youtube.com'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
#   - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

<!-- {{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}} -->

<!-- Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://wowchemy.com/docs/content/writing-markdown-latex/). -->

# Abstract
Multi-modal image registration is an essential step for many medical image analysis applications. Recent advances in multi-modal image registration rely on image-to-image translation to achieve good performance. However, the performance is still limited owing to the poor use of complementary regularization between image registration and translation, which is able to simultaneously enhance both parts’ accuracy. To this end, we propose CoCycleReg, a novel method that formulates image registration and translation in a Collaborative Cycle-consistency manner. Instead of dividing into two discrete stages, we unify the image registration and translation via cycle-consistency in an end-to-end training process, such that each part can benefit from the other one. To ensure the deformation fields’ reversibility in the cycle, we extensively introduce a novel dual-head registration network, consisting of one single backbone to extract the features and two heads to respectively predict the deformation fields. The experiments on T1-T2(MRI) and CT-MRI datasets validate that the proposed CoCycleReg surpasses the other state-ofthe-art conventional and deep learning approaches comprehensively considering the speed, accuracy, and regularity of deformation fields. In the ablation analysis, a method that sets the cycle-consistency Corresponding authors at: Department of Computer Science at School of Informatics, Xiamen University, Xiamen 361005, Chinaconstraints of registration and image-to-image translation separately is compared, and the results demonstrate the effectiveness of collaborative cycle-consistency. In addition, the improvement of image-to-image translation is also verified in further analysis. The code is publicly available at https://github.com/DopamineLcy/cocycle-reg/.
{style="text-align: justify;"}