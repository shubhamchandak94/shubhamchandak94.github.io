---
layout: page
title: Research Projects
---

Here are some of the research projects I have participated in over the years, please check out the publications page for the corresponding papers.

- **Error correction for DNA storage** _(Ph.D. research)_  
  Stanford University  

  <img src="/img/research/dna_storage.png" alt="Error correcting codes for DNA storage" max-height="966" max-width="2164" width="100%">

  **Introduction:** DNA as a storage medium can provide high storage density and long-term durability, and hence can be an alternative for traditional magnetic/semiconductor-based storage media in the near future. However, the DNA synthesis and sequencing processes are expensive and noisy, and there is a need to design optimized encoding/decoding schemes with error correction for reliable data recovery. In particular, nanopore sequencing provides low cost, portable and real-time solution at the expense of higher error rates making error correction coding critical.

  - We studied the tradeoff between the writing and reading costs involved in DNA-based storage and propose a practical [scheme](https://github.com/shubhamchandak94/LDPC_DNA_storage) based on LDPC codes to achieve an improved tradeoff between these quantities.
  - For nanopore sequencing based DNA storage, we proposed a novel [approach](https://github.com/shubhamchandak94/nanopore_dna_storage) which overcomes the high error rates in nanopore sequencing by exploiting the soft information available in the raw signals.
  - Check out my [talk](https://www.youtube.com/watch?v=7ki2QcSg59c) at ISMB/ECCB 2019 to get a high-level overview of this work.

- **FASTQ compression** _(Ph.D. research)_  
  Stanford University  

  <img src="/img/research/fastq.png" alt="Genome sequencing" max-height="782" max-width="2736" width="100%">

  **Introduction:** Next generation sequencing of genomes produces large amounts of data in the form of short reads which are stored in FASTQ files. For a typical experiment, these files can be 100s of GBs large.

  - Performed theoretical analysis of the problem by computing upper bounds on the entropy of reads and developed [HARC](https://github.com/shubhamchandak94/HARC/), a tool to compress reads with and without preserving their order, achieving near-optimal compression ratios.
  - Improved upon HARC to develop [SPRING](https://github.com/shubhamchandak94/SPRING/), a practical tool to compress single and paired-end FASTQ files, supporting a variety of modes and features.
  - Work published in _Bioinformatics_.
  - Check out my [talk](https://www.youtube.com/watch?v=OCngQbmyKow) at ISMB/ECCB 2019 to get an overview of this work.
  - Currently working to integrate parts of SPRING with [genie](https://github.com/mitogen/genie), an open-source [MPEG-G](https://mpeg-g.org/) codec.

- **Time series data compression** _(Ph.D. research)_  
  Stanford University (in collaboration with Siemens)

  <img src="/img/research/lfzip.png" alt="Genome sequencing" max-height="386" max-width="2480" width="100%">

  Time series data compression is increasing becoming critical with the large volumes of data produced by IoT devices and sensors. Lossy compression is often appropriate for such datasets due to the presence of noise and can lead to huge compression gains without sacrificing accuracy of downstream analysis.  
  We developed [LFZip](https://github.com/shubhamchandak94/LFZip), an error-bounded lossy compressor for multivariate floating-point time series data based on  the prediction quantization-entropy coder framework. LFZip benefits from improved prediction using linear models and neural networks and outperforms the existing state-of-the-art error-bounded lossy compressors on several time series datasets.


- **Applications of Gröbner Basis** _(B. Tech. Project)_  
  August 2015 - May 2016  
  IIT Bombay  
  _Guide: Prof. Harish Pillai_  

  **Introduction:** Gröbner Basis is a computational tool for studying ideals in multivariate polynomial rings. It has applications in Commutative Algebra, Integer Optimization, Control Systems and other areas.

  - Studied the basic Gröbner basis theory and its connections to convex polytopes, toric ideals, integer programming and regular triangulations.
  - Obtained new relations for the pole placement problem using state feedback in single input systems by interpreting results from Gröbner bases in the control theoretic setting.
  - Extended the formulae to multi-input system using Gröbner basis and linear algebra.

  [[report](/reports/btp2_report.pdf)]

- **Elliptic Curve Cryptography for IoT** _(Summer internship)_  
  May 2015 - July 2015  
  Massachusetts Institute of Technology    
  _Guide: Prof. Anantha Chandrakasan_

  **Introduction:** Securing the Internet of Things is a major challenge due to the area and power constraints. Elliptic Curve Cryptography (ECC) is the most suitable public key scheme for IoT due to the small key sizes. Our aim was to design a ECC scalar multiplication processor for constrained applications.  

  - Implemented Datagram Transport Layer Security (DTLS) handshake on low power ARM Cortex-M0+ processor using Arduino WiFiShield to identify the bottleneck operations during secure communication.
  - Surveyed existing low-area/energy implementations of ECC and studied Koblitz curves which have a Frobenius endomorphism allowing faster scalar multiplication using τ-adic representation.
  - Designed an integer to τ -adic converter which was absent from the existing low-area implementations, with only a marginal increase in area by reusing the registers and ALU.
  - Work published in _IEEE Journal of Solid-State Circuits_.

- **Functional Electrical Stimulation - Numerical Analysis** _(Summer internship)_  
  May 2014 - July 2014  
  Oxford Brookes University, Oxford, UK      
  _Guides: Dr. Cristiana Sebu, Oxford Brookes University, UK; Dr. Brian Andrews, Nuffield Department of Surgical Sciences, University of Oxford, UK_

  **Introduction:** Functional Electrical Stimulation (FES) is a technique that uses electric currents to activate nerves, helping restore function in people with disabilities. The challenge is to design electrodes which produce high nerve activation at desired depth while keeping surface current densities low.  

  - _Concentric Electrodes_: Formulated Laplace equation for three-layer body model as integral equations using Hankel transform. The Nyström method with Gauss-Legendre quadrature was used to solve these equations. The Fourier-Bessel series was introduced to evaluate oscillatory integrals. See the analysis [here](/reports/brookes_two_layer.pdf) and [here](/reports/brookes_three_layer.pdf).  
  - _Non-concentric Electrodes_: For square and other electrodes, a Finite Element model was solved using EIDORS software on MATLAB.
  - Compared various electrode configurations for safety and effectiveness using MATLAB simulations. See the results [here](/reports/brookes_simulations.pdf).

- **Spiking Neural Networks**
  May 2013 - December 2013    
  IIT Bombay        
  _Guide: Prof. Bipin Rajendran_

  **Introduction:** Spiking Neural Networks (SNNs) can represent complex temporal relations between the input and output. Our aim was to study and implement algorithms for training of SNNs inspired by the brain.  

  - Studied spiking neuron models as well as Artificial Neural Networks.  
  - Studied and implemented ReSuMe, a supervised learning technique for SNNs based on Spike Timing Dependent Plasticity (STDP), on MATLAB.
