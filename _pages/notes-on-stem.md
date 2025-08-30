---
permalink: /notes-on-stem/
title: "Notes on STEM"
excerpt: "This page contains notes related to Science, Technology, Engineering, and Mathematics (STEM)."
author_profile: false
---

<span class='anchor' id='notes-on-stem'></span>

This page is intended to provide general guidance for undergraduate students in physics, biomedical engineering, or related STEM fields who are interested in medical physics. In general, the mathematical and physical foundations required for medical physics overlap only partially with those of a typical physics undergraduate curriculum—one might even say that the Dice–Sørensen coefficient (DSC) between the two is less than 1, that is,  

\[
\text{DSC}(MP, P) = \frac{2 |MP \cap P|}{|MP| + |P|} < 1
\]

Given that medical physics encompasses various topics, including radiation, imaging, and nuclear medicine, different emphases may arise depending on personal interests. For radiation-focused paths, nuclear physics and dosimetry are essential; for imaging-focused paths, image processing and related mathematical methods are more important. However, based on my own experience and observations of peers who have achieved remarkable results, there is no harm in developing a broad horizon and cultivating strong problem-solving fundamentals, especially at the early stages of one’s career.

As L. D. Landau once advised students of physics:

> “As to your question concerning the study of theoretical physics, I can state only that it is necessary to learn ALL its main branches, and the sequence of study is dictated by their mutual relationship. As a method of study, I can only emphasize that you must perform all the calculations by yourself, and must not leave it to the authors of the books you have read.”  
> – *L. D. Landau, cited in E. M. Lifshitz, Am. J. Phys. 45, 415 (1977); doi: 10.1119/1.10828*

Nevertheless, the theoretical foundations outlined below reflect only my personal experience and biases. They are offered tentatively, for readers to consider at their own discretion.

# Fundamental Commonly Covered in Undergraduate

- **Mathematical methods in physics**
  - ODEs and PDEs, Contour Integral, Green’s functions, and variational methods. Special functions like Legendre, Bessel, and spherical harmonics appear often. Group theory and Lie algebra are also helpful for advanced theory.
  - [*Hassani*](https://link.springer.com/book/10.1007/978-3-319-01195-0) is good for a general overview and advanced details. Numerical methods texts are more practical.

- **Computational methods**
  - Monte Carlo simulation ([Geant4](https://geant4.web.cern.ch/), [FLUKA](http://www.fluka.org/fluka.php?)) for radiation transport, finite element methods(COMSOL, ANSYS) for solving EM field problems, and numerical techniques for dose calculation.
  - For practical applications, open-source toolkits and software manuals are often more useful.

- **Quantum mechanics**
  - Knowledge until second quantization (so-called advanced quantum mechanics) is enough. Most problems in medical physics deal with atomic-level fine-structure effects, such as spin-orbit coupling and relativistic corrections. QFT is unnecessary unless calculating exact reaction cross-sections, secondary electron production in radiotherapy or higher-order corrections in positron annihilation processes.
  - [*Griffiths*](https://www.cambridge.org/highereducation/books/introduction-to-quantum-mechanics/990799CA07A83FC5312402AF6860311E#overview), [*Sakurai*](https://www.cambridge.org/highereducation/books/modern-quantum-mechanics/DF43277E8AEDF83CC12EA62887C277DC#overview) are fine for beginners, refer to [*Cohen-Tannoudji*](https://www.wiley.com/en-us/Quantum+Mechanics%2C+Volume+1%3A+Basic+Concepts%2C+Tools%2C+and+Applications%2C+2nd+Edition-p-9783527822713) for details.

- **Electrodynamics**
  - Calculation of EM fields, relativistically charged particle dynamics, wave propagation in biological tissues and detectors. QED is not necessary, though familiarity with Feynman diagrams can be beneficial.
  - Begin with [*Griffiths*](https://www.cambridge.org/highereducation/books/introduction-to-electrodynamics/3AB220820DBB628E5A43D52C4B011ED4#overview), advance to [*Jackson*](https://www.wiley.com/en-au/Classical+Electrodynamics%2C+3rd+Edition-p-9780471309321) and [*Zangwill*](https://www.cambridge.org/highereducation/books/modern-electrodynamics/E5448C70CBF3651B2056F28EBF859AE9#overview).

# Beyond the Undergraduate

- **Nuclear physics**
  - Basic nuclear models (liquid drop, shell model and collective model), decay modes of radioactive nuclides ($α, β^+, β^−, γ$) and cross-section calculations of nuclear reactions.
  - [*Martin*](https://www.wiley.com/en-us/Nuclear+and+Particle+Physics%3A+An+Introduction%2C+3rd+Edition-p-9781119344612) and [*Krane*](https://www.wiley.com/en-us/Introductory+Nuclear+Physics%2C+3rd+Edition-p-9780471805533) are good starting points. [*Tina Potter’s slides*](https://www.hep.phy.cam.ac.uk/~chpotter/particleandnuclearphysics/mainpage.html) provide clear explanations and useful insights. For more details, refer to [*Blatt & Weisskopf*](https://link.springer.com/book/10.1007/978-1-4612-9959-2) for formal scattering theory.

- **Radiation physics**
  - Electron, photon, neutron interaction with matter.
  - [*Turner*](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527616978) and [*Hooshang Nikjoo*](https://www.routledge.com/Interaction-of-Radiation-with-Matter/Nikjoo-Uehara-Emfietzoglou/p/book/9780367866020?srsltid=AfmBOor8xnXQC1WBWkicRN74gtG5SBA1yQae0BHI2zQaCsMWPPs2T-Ny) are helpful, refer to [*Radiation Physics for Medical Physicists*](https://link.springer.com/book/10.1007/978-3-319-25382-4) for details.

- **Detection of radiation**
  - Principles of radiation detection, including gas-filled detectors, scintillators, and semiconductor detectors. Concepts like energy resolution, efficiency, dead time, and statistical uncertainty are crucial. Pulse processing and spectroscopy methods are also important for practical applications.
  - [*Knoll*](https://www.wiley.com/en-ae/Radiation+Detection+and+Measurement%2C+4th+Edition-p-9780470131480), [*Attix*](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527617135) and [*Fundamentals of Ionizing Radiation Dosimetry*](https://www.wiley.com/en-us/Fundamentals+of+Ionizing+Radiation+Dosimetry-p-9783527409211).

- **Physics of radiotherapy**
  - Intensity-Modulated Radiation Therapy (IMRT), Volumetric Modulated Arc Therapy (VMAT), Image-Guided Radiation Therapy (IGRT), Stereotactic Body Radiation Therapy (SBRT), Boron Neutron Capture Therapy (BNCT), Proton Therapy, and Heavy Ion Therapy.
  - [*The Physics of Radiotherapy X-Rays and Electrons 3rd Edition*](https://medicalphysics.org/SimpleCMS.php?content=bookpage.php&isbn=9781951134105) and [*Khan’s The Physics of Radiation Therapy*](https://shop.lww.com/Khan-s-The-Physics-of-Radiation-Therapy/p/9781496397522?srsltid=AfmBOopw7KJsy68Iq6t5fNmViGW7WDQIXC6WdX8PdLDcxhLL__zHAxzC) provide a comprehensive overview.
  - AAPM Task Group reports and ICRU reports serve as essential clinical references.

- **Physics of medical imaging**
  - Computed Tomography (CT), Magnetic Resonance Imaging (MRI), Positron Emission Tomography-Computed Tomography (PET-CT), Ultrasound Imaging and other related imaging modalities.
  - [*The Essential Physics of Medical Imaging, 3rd Edition*](https://pubmed.ncbi.nlm.nih.gov/28524933/), [*Fundamental Mathematics and Physics of Medical Imaging*](https://doi.org/10.1201/9781315368214) and [*Medical Imaging Physics, 4th Edition*](https://www.wiley.com/en-us/Medical+Imaging+Physics%2C+4th+Edition-p-9780471461135).

- **Radiobiology and radiation protection**
  - Linear-Quadratic (LQ) model, bystander effects, ALARA principle and shielding calculations.
  - [*Radiobiology for the Radiologist 8th Edition*](https://shop.lww.com/Radiobiology-for-the-Radiologist/p/9781496335418?srsltid=AfmBOoo02iTJHtt_TgiT5JeADx5hU9Ajv1sa-huxtqe2FC83wHVL05ui).

# Cheatsheets, Notes and Summaries (Feedback and typo corrections are welcome!)
- **Electromagnetism:**  [PDF](https://louis-qiuyulu.github.io/CheatSheet-EM.pdf)
- **Nuclear physics:**  [PDF](https://louis-qiuyulu.github.io/summary-of-NP.pdf) 
- **Radiation physics:**  [PDF](https://louis-qiuyulu.github.io/CheatSheet-RP.pdf)
- **Medical imaging:**  [PDF](https://louis-qiuyulu.github.io/summary-of-MI.pdf)
- **Physics of radiotherapy:**  [PDF](https://louis-qiuyulu.github.io/summary-of-RT.pdf)
- **Radiobiology and radiation protection:**  [PDF](https://www.youtube.com/watch?v=dQw4w9WgXcQ)

---

## License  
These notes are licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).  

[![CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
