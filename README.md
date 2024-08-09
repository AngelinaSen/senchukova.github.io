# Researcher / Data Scientist

[GitHub](https://github.com/AngelinaSen) | [Google Scholar](https://scholar.google.com/citations?hl=en&user=sghAn8cAAAAJ) | [LinkedIn](https://www.linkedin.com/in/senchukova/)

I am a doctoral researcher based in Helsinki, Finland. As a part of the [Uncertainty Quantification and Inverse Problems](https://www.lut.fi/en/research-groups/uncertainty-quantification-and-inverse-problems) group at LUT University, I work on Bayesian inverse problems under the supervision of [Prof. Lassi Roininen](https://www.lut.fi/fi/profiilit/lassi-roininen) and [Prof. Tapio Helin](https://www.lut.fi/fi/profiilit/tapio-helin). 

I have been mostly involved in the development of flexible priors, which are used to promote specific behavior in reconstructions and enhance the reconstruction quality when the data is limited or corrupted by noise. Applications include X-ray computed tomography, image deblurring, and signal deconvolution. 

I am defending my doctoral thesis this autumn (tentatively on October 4, 2024) and seeking full-time employment in the Helsinki metropolitan area. My professional interests include data science, machine learning, and software development.


## Education 
* **PhD _in Computational Science_** @ LUT University, Finland (_expected graduation: November 2024_)
  
  Thesis: _"Flexible priors for rough feature reconstruction in Bayesian inversion"_   

* **MSc _in Computational Engineering_** @ LUT University, Finland (_July 2020_)

  Thesis: _"Learned image reconstruction in X-ray computed tomography"_ 

* **BSc _in Applied Mathematics and Informatics_** @ Southern Federal University, Russia (_June 2018_)

  Thesis: _"Boundedness and invertibility of convolution operators on the infinite dihedral group"_ (in Russian)

## Work Experience 
**Junior Researcher @ LUT University (_January 2021 - Present_)**

* _Edge-preserving inversion with Bayesian neural networks priors_
  
  The project involved developing priors for recovering sharp features in inverse problems such as X-ray computed tomography, where the objects of interest usually have a blocky structure. We suggested building the priors in a functional space-based manner using probabilistic (Bayesian) neural networks with parameters drawn from the Student's _t_ distribution.

  __Tech Stack__: `Python`, `PyTorch`, `SciPy`, `MCMC methods`

* _Flexible Student's t priors based on Gaussian scale mixtures_ [[preprint](https://arxiv.org/pdf/2403.13665)]
  
  The project aimed at constructing priors capable of recovering both sharp or smooth features in the reconstructions. To this end, we combined the Markov random field structure and Student's t distribution, whose behavior can be controlled by the degrees of freedom parameter.
  By including the degrees of freedom parameter in the hierarchical formulation of the model, we were able to automatically tune it based on the available data.

  __Tech Stack__: `Python`, `NumPy`, `Pandas`, `scikit-sparse`, `arviz`, `NUTS`, `Gibbs sampler`

* _X-ray imaging for sawmills_ [[journal article](https://doi.org/10.1007/s10851-023-01167-6), [GitHub repo](https://github.com/AngelinaSen/geometry_parameter_estimation)]
  
  The main goal of the project was to improve the sawmill workflow using non-invasive sensing through the X-ray computed tomography of logs. I developed a method for estimating unknown parameters of fan-beam X-ray geometry using the calibration object.

  __Tech Stack__: `OpenCV Python library`, `ASTRA Tomography Toolbox`, `SciPy`


## Publications 
[1] __A. Senchukova__, F. Uribe, L. Roininen. Bayesian inversion with Student's t priors based on Gaussian scale mixtures. arXiv [preprint](https://arxiv.org/pdf/2403.13665), 2024.

[2] __A. Senchukova__, J. Suuronen, J. Heikkinen, L. Roininen. Geometry parameter estimation for sparse X-ray log imaging. Journal of Mathematical Imaging and Vision, 2024, 66(2): 154-166. [doi](https://doi.org/10.1007/s10851-023-01167-6)

[3] S. Springer, A. Glielmo, __A. Senchukova__, T. Kauppi, J. Suuronen, L. Roininen, H. Haario, A. Hauptmann. Reconstruction and segmentation from sparse sequential X-ray measurements of wood logs. Applied Mathematics for Modern Challenges, 2023, 1(1): 1-20. [doi](https://doi.org/10.3934/ammc.2023002)

[4] V. Deundyak, D. Leonov, __A. Senchukova__. Symbolic calculation and invertibility of convolution operators on the infinite dihedral group. Mathematical Physics and Computer Modeling, 2020, 23(3). [doi](https://mp.jvolsu.com/index.php/en/archive-en/389-mathematical-physics-and-computer-simulation-2020-vol-23-no-3/mathematics-and-mechanics/929-deundyak-v-m-leonov-d-a-senchukova-a-a-symbolic-calculation-and-invertibility-of-convolution-operators-on-the-infinite-dihedral-group)

## Talks & Meetings
- Poster presenter @ [Satellite workshop to ISBA world meeting](https://www.usi.ch/en/feeds/25999), Lugano, Switzerland (_June 25-28, 2024_)
- [Talk](https://meetings.siam.org/sess/dsp_programsess.cfm?SESSIONCODE=78220) @ SIAM Conference on Uncertainty Quantification (UQ24), Trieste, Italy (_February 27-March 1, 2024_)
- Participant @ [Autumn school in Bayesian Statistics](https://bayesatcirm.github.io/2023/), CIRM, Marseille, France (_October 30-November 3, 2023_)
- Talk @ 11th Applied Inverse Problems Conference, Göttingen, Germany (_September 3-8, 2023_)
- Talk @ ECCOMAS Young Investigators Conference 2023, Porto, Portugal (_June 19-21, 2023_)
- Poster presenter @ [SFB 1294 Spring School](https://www.sfb1294.de/events/event/spring-school-2023), Germany (_March 20-24, 2023_)
- Participant @ [Bayes Comp 2023](https://bayescomp2023.com), Levi, Finland (_March 12-17, 2023_)
- Visit & [Talk](https://www.sfb1294.de/events/event/two-prior-models-for-edge-preserving-bayesian-inversion) @ Collaborative Research Centre SFB 1294 on Data Assimilation, University of Potsdam, Potsdam, Germany. (_October 25-November 4_, 2022, with Prof. Dr. J. de Wiljes)

## Research Grants 
- Awarded a research grant for doctoral studies from [the Väisälä Fund](https://acadsci.fi/en/about-the-academy/funds-and-foundations/vaisala-foundation/) of the Finnish Academy of Science and Letters worth 70 500 EUR (_2022-2024_).

## Teaching Experience
- **Teaching assistant** in _Functional Analysis_ (_2021_, with Tapio Helin), _Simulation and System Dynamics_ (_2020-2021_, with Heikki Haario), and _Probabilistic Simulation_ (_2022-2024_, with Tomás Soto) courses at LUT University.
