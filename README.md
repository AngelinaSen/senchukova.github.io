# Researcher / Data Scientist

[GitHub](https://github.com/AngelinaSen) | [Google Scholar](https://scholar.google.com/citations?hl=en&user=sghAn8cAAAAJ) | [LinkedIn](https://www.linkedin.com/in/senchukova/)

### About Me

I am a doctoral researcher based in Helsinki, Finland. As a part of the [Uncertainty Quantification and Inverse Problems](https://www.lut.fi/en/research-groups/uncertainty-quantification-and-inverse-problems) group at LUT University, I work on Bayesian inverse problems under the supervision of [Prof. Lassi Roininen](https://www.lut.fi/fi/profiilit/lassi-roininen) and [Prof. Tapio Helin](https://www.lut.fi/fi/profiilit/tapio-helin). 

My research evolves around the development of flexible priors for inverse problems, which are used to promote specific behavior in reconstructions and enhance the reconstruction quality in cases when the data is limited or corrupted by noise. Applications include industrial X-ray computed tomography, image deblurring, and signal processing. 

I am defending my doctoral thesis this autumn (tentatively on October 4, 2024) and seeking full-time employment in the Helsinki metropolitan area. My professional interests include data science, machine learning, and software development.

### About my Research: Bayesian Inverse Problems

Solving inverse problems, we aim at reconstructing a quantity of interest from its noisy indirect measurements. A wide-known example is X-ray computed tomography used for non-invasive medical diagnostics, where the goal is to obtain an image of the patient's  internal organs using the intensity attenuation of X-ray beams passing through the body. Inverse problems are tricky to solve as the solution may not exist, may not be unique, or may not depend continuously on the measurement data (this property is called _ill-posedness_). The Bayesian approach provides a way to obtain stable solutions to inverse problems by treating all the unknowns as random variables and encoding our prior knowledge of the unknown in the form of the prior distribution. Within the Bayesian framework, the solution is formulated as a posterior distribution rather than a single estimate, which also allows for quantifying the uncertainty, that is, estimating how reliable the obtained result is. 

## Education 
* **PhD _in Computational Science_** @ LUT University, Finland (_expected graduation: November 2024_)
  
  Thesis: _"Flexible priors for rough feature reconstruction in Bayesian inversion"_   

* **MSc _in Computational Engineering_** @ LUT University, Finland (_July 2020_)

  Thesis: [_"Learned image reconstruction in X-ray computed tomography"_](https://urn.fi/URN:NBN:fi-fe2020062445578)

* **BSc _in Applied Mathematics and Informatics_** @ Southern Federal University, Russia (_June 2018_)

  Thesis: _"Boundedness and invertibility of convolution operators on the infinite dihedral group"_

## Work Experience 
**Junior Researcher @ LUT University (_January 2021 - Present_)**

* _Flexible Student's t priors based on Gaussian scale mixtures_ [[preprint](https://arxiv.org/pdf/2403.13665)]
  
  Within the project, I developed a class of priors combining the Markov random field structure with Student's _t_ distribution. The prior demonstrates the flexibility and can be used for reconstructing both sharp (piecewise constant) and smooth features in the solution. This flexibility is achieved by treating the degrees of freedom parameter of the _t_ distribution as a hyperparameter and learning it from the data. Hence, the method eliminates the complicated hand-tuning of the degrees of freedom parameter and allows its automatic inference. To simplify the characterization of the multimodal posterior distribution, I employed the Gaussian scale mixture representation of Student's _t_ distribution, which allowed for the application of the efficient Gibbs sampler for obtaining the solution. The priors were tested numerically for smooth and sharp data and showed good performance when compared with the other popular priors used for inverse problems, such as Laplace and Cauchy difference priors. 
  
  __Tech Stack__: `Python`, `NumPy`, `Pandas`, `scikit-sparse`, `arviz`, `Linux`, `NUTS`, `Gibbs sampler`

* _Solving inverse problems with Bayesian neural networks priors_ [[GitHub repo](https://github.com/AngelinaSen/bnn_priors)]

  For this research project, I implemented priors in a functional space-based manner using probabilistic (Bayesian) neural networks with parameters drawn from the Student's _t_ distribution. The advantage of this approach (as compared to discretization-based priors) is that the result does not depend on the size of the discretization mesh used for the problem. I applied the suggested priors to several signal deconvolution problems and explored the methods to improve the posterior sampling, as the posterior distribution has a very complicated landscape being multidimensional and multimodal. 

  __Tech Stack__: `Linux`, `Python`, `PyTorch`, `SciPy`, `MCMC methods`, `NUTS`, `preconditioned Crank–Nicolson sampler`

* _Sparse X-ray imaging for sawmills_ [[journal article](https://doi.org/10.1007/s10851-023-01167-6), [GitHub repo](https://github.com/AngelinaSen/geometry_parameter_estimation)]
  
  This project was done in collaboration with [Finnos Oy](https://www.finnos.fi/en/), a Finnish company developing X-ray scanners applied in the sawmill industry for wood log sorting. As a part of the project, I was working on the reconstruction of the inner structure of the wood logs from their X-ray measurements provided by Finnos. As the geometry of the scanning equipment was partially unknown, I developed a method for estimating unknown parameters of fan-beam X-ray geometry using the calibration object. After identifying the geometry parameters, I applied Bayesian inversion with Cauchy difference priors to obtain reconstructions of wood logs. As only a limited amount of X-ray data was available, the use of Cauchy priors allowed for better preservation of sharp features in the reconstructions compared to the traditional reconstruction techniques. The reconstructions were further used to detect log features, such as tree knots and rotten parts, to optimize the strategy used for sawing logs into lumber and, therefore, reduce waste and enhance the sustainability of sawmills.

  __Tech Stack__: `Linux`, `OpenCV Python library`, `ASTRA Tomography Toolbox`, `SciPy`, `Matlab`


## Publications 
[1] __A. Senchukova__, F. Uribe, L. Roininen. [Bayesian inversion with Student's t priors based on Gaussian scale mixtures](https://arxiv.org/pdf/2403.13665). arXiv preprint, 2024.

[2] __A. Senchukova__, J. Suuronen, J. Heikkinen, L. Roininen. [Geometry parameter estimation for sparse X-ray log imaging](https://doi.org/10.1007/s10851-023-01167-6). Journal of Mathematical Imaging and Vision, 2024, 66(2): 154-166.

[3] S. Springer, A. Glielmo, __A. Senchukova__, T. Kauppi, J. Suuronen, L. Roininen, H. Haario, A. Hauptmann. [Reconstruction and segmentation from sparse sequential X-ray measurements of wood logs](https://doi.org/10.3934/ammc.2023002). Applied Mathematics for Modern Challenges, 2023, 1(1): 1-20.

[4] V. Deundyak, D. Leonov, __A. Senchukova__. [Symbolic calculation and invertibility of convolution operators on the infinite dihedral group](https://mp.jvolsu.com/index.php/en/archive-en/389-mathematical-physics-and-computer-simulation-2020-vol-23-no-3/mathematics-and-mechanics/929-deundyak-v-m-leonov-d-a-senchukova-a-a-symbolic-calculation-and-invertibility-of-convolution-operators-on-the-infinite-dihedral-group). Mathematical Physics and Computer Modeling, 2020, 23(3): 60-75.

## Talks & Meetings
- Poster presenter @ [Satellite workshop to ISBA world meeting](https://www.usi.ch/en/feeds/25999), Lugano, Switzerland (_June 25 - 28, 2024_)
- [Talk](https://meetings.siam.org/sess/dsp_programsess.cfm?SESSIONCODE=78220) @ SIAM Conference on Uncertainty Quantification (UQ24), Trieste, Italy (_February 27 - March 1, 2024_)
- Participant @ [Autumn school in Bayesian Statistics](https://bayesatcirm.github.io/2023/), CIRM, Marseille, France (_October 30 - November 3, 2023_)
- Talk @ 11th Applied Inverse Problems Conference, Göttingen, Germany (_September 3 - 8, 2023_)
- Talk @ ECCOMAS Young Investigators Conference 2023, Porto, Portugal (_June 19 - 21, 2023_)
- Poster presenter @ [SFB 1294 Spring School](https://www.sfb1294.de/events/event/spring-school-2023), Germany (_March 20 - 24, 2023_)
- Participant @ [Bayes Comp 2023](https://bayescomp2023.com), Levi, Finland (_March 12 - 17, 2023_)
- Visit & [Talk](https://www.sfb1294.de/events/event/two-prior-models-for-edge-preserving-bayesian-inversion) @ Collaborative Research Centre SFB 1294 on Data Assimilation, University of Potsdam, Potsdam, Germany. (_October 25 - November 4_, 2022, with Prof. Dr. J. de Wiljes)
- Participant @ [DTU Workshop: Imaging With Uncertainty Quantification](https://people.compute.dtu.dk/pcha/CUQI/IUQworkshop.html), Helsingør, Denmark (_September 26 - 29, 2022_)
- Participant @ Summer School on Applied Harmonic Analysis and Machine Learning, Genova, Italy (_September 5 - 9, 2022_)
- Online talk @ SIAM Conference on Uncertainty Quantification (UQ22), Atlanta, Georgia, U.S. (_April 12 - 15, 2022_)
- Visit @ KTH Royal Institute of Technology, Stockholm, Sweden (_October 5 - November 2, 2021_, with Prof. Ozan Öktem)

## Research Grants 
Awarded a **research grant for doctoral studies** from [the Väisälä Fund](https://acadsci.fi/en/about-the-academy/funds-and-foundations/vaisala-foundation/) of the Finnish Academy of Science and Letters worth 70 500 EUR (_2022-2024_).

## Teaching Experience
**Teaching assistant** for the courses at LUT University:  
* _Functional Analysis_ (_2021_, with Tapio Helin)
* _Simulation and System Dynamics_ (_2020 - 2021_, with Heikki Haario)
* _Probabilistic Simulation_ (_2022 - 2024_, with Tomás Soto)
