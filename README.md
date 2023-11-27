### 👋 Hi there 
I am a deep learning/machine learning engineer and have experience with working in startups as deep learning and computer vision developer👨‍💻. Interested in making life better by letting machines learn. Fascinated about AGI (artificial general intelligence). Highly motivated for solving problems in real applications.


- 🔭 Professional experience with technology stacks with TensorFlow, Keras, PyTorch, OpenCV, Numpy, AWS, GCP, Docker, testing, CI/CD pipelines.
- 🔭 Fluent in Python.
- 🍔 Contributor to the open source medical imaging framework [TorchIO](https://torchio.readthedocs.io/#).
- ⚡ Worked for startups in de sports analytics and medical imaging sector.
- 💬 Already working with neural networks and deep learning since 2010. 

### Projects

#### Real time 3D player and ball tracking
For a startup in the football industry I worked on real-time autonomous player and ball tracking. This product was used on the highest level in the Netherlands and in England. 

To make this work we developed fast deep learning based player and ball detections algorithms based on YOLO (You Only Look Once). 

![github](https://raw.githubusercontent.com/dmus/about-me/main/football.png)

The next step was classifying all detections. Is there a jersey number visible and if yes, which number? For this step a lot of labeled data is needed, also for the sparse numbers. Some smart methods were used here to handle this imbalance in the data. 

Besides the jersey number the team has to be classified. The challenge here is that is has to work for all kind of jerseys, even for teams and outfits never seen before. A powerful feature representation was learned, which could be used to say if jerseys are from the same team or not. In combination with clustering algorithms, this yielded a powerful team classifier.

Other components involved are the linking of detections that belong the the same player or the same ball and the translation from image coordinates to world coordinates in 3D. This involves registration algorithms for the field, both deep learning and non deep learning based.

![github](https://raw.githubusercontent.com/dmus/about-me/main/teaser.png)

#### Synthetic CT generation
For a startup in the medical industry I worked on generating synthetic CT images from MRI images to avoid harmful radiation. This is used in several hospitals around the world. This work also requires multiple deep learning components. A challenging aspect is that medical 3D images are very large and cannot be loaded completely on (most) GPUs.

Localization and segmentations of bones are needed to detect the rigid parts of an image. First bones are localized and then a region around the detected landmark is cropped and segmented.

![github](https://raw.githubusercontent.com/dmus/about-me/main/landmarks.png)

A combination of deformable and nondeformable registration algorithms is used to generate high quality paired data that can be used for supervised learning algorithms.

3D image to image deep learning algorithms are used to generate the synthetic CTs. Multiple methods are developed, based on CNNs (convolutional neural networks), GANs (Generative Adverserial Neural Networks), PerceiverIO (transformed based neural networks) and diffusion models.

![github](https://raw.githubusercontent.com/dmus/about-me/main/synct.png)

Also the evaluation is an important part. To do this I developed surface distance metrics and visualizations to measure and show distances between the bones on the original CT and the synthetic CT.

![github](https://raw.githubusercontent.com/dmus/about-me/main/eval.png)

#### Generating robotic manipulation trajectories
As deep learning research intern at IBM I worked on a deep learning project for generating manipulation trajectories for a robot arm. This work involved handling multimodal input (point clouds and text) and generating a trajectory in an autoregressive way.

<hr />

### Visitor count
<img src="https://profile-counter.glitch.me/dmus/count.svg" />

### 📫 Reach me at 
[![Linkedin](https://i.stack.imgur.com/gVE0j.png) LinkedIn](https://www.linkedin.com/in/derkmus/)
