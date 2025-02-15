---
permalink: /notes-on-stem/
title: "Notes on STEM"
excerpt: "This page contains notes related to Science, Technology, Engineering, and Mathematics (STEM)."
author_profile: false
---

<span class='anchor' id='notes-on-stem'></span>

# Fundamental Topics Commonly Covered in Undergraduate Physics

- **Mathematical methods in physics**
  - Partial differential equations, Green’s functions, and variational methods. Special functions like Legendre, Bessel, and spherical harmonics appear often but usually in pre-tabulated or numerically evaluated forms.
  - [*Hassani*](https://link.springer.com/book/10.1007/978-3-319-01195-0) is good for a general overview and advanced details. Numerical methods texts are more practical.

- **Computational methods**
  - Monte Carlo simulation ([Geant4](https://geant4.web.cern.ch/), [FLUKA](http://www.fluka.org/fluka.php?)) for radiation transport, finite element methods(COMSOL, ANSYS) for solving EM field problems, and numerical techniques for dose calculation.
  - For practical applications, open-source toolkits and software manuals are often more useful than standard textbooks.

- **Quantum mechanics**
  - Knowledge until second quantization (so-called advanced quantum mechanics) is enough. Most problems in medical physics deal with atomic-level fine-structure effects, such as spin-orbit coupling and relativistic corrections. QFT is unnecessary unless calculating exact reaction cross-sections, secondary electron production in radiotherapy or higher-order corrections in positron annihilation processes (e.g., angular distribution of annihilation photons).
  - [*Griffiths*](https://www.cambridge.org/highereducation/books/introduction-to-quantum-mechanics/990799CA07A83FC5312402AF6860311E#overview), [*Sakurai*](https://www.cambridge.org/highereducation/books/modern-quantum-mechanics/DF43277E8AEDF83CC12EA62887C277DC#overview) are fine for beginners, refer to [*Cohen-Tannoudji*](https://www.wiley.com/en-us/Quantum+Mechanics%2C+Volume+1%3A+Basic+Concepts%2C+Tools%2C+and+Applications%2C+2nd+Edition-p-9783527822713) for details.

- **Electrodynamics**
  - Calculation of EM fields, relativistically charged particle dynamics, wave propagation in biological tissues (e.g., $B_1$ field distribution in MRI, RF heating). QED is not necessary, though familiarity with Feynman diagrams can be beneficial for those interested.
  - Begin with [*Griffiths*](https://www.cambridge.org/highereducation/books/introduction-to-electrodynamics/3AB220820DBB628E5A43D52C4B011ED4#overview), advance to [*Jackson*](https://www.wiley.com/en-au/Classical+Electrodynamics%2C+3rd+Edition-p-9780471309321) and [*Zangwill*](https://www.cambridge.org/highereducation/books/modern-electrodynamics/E5448C70CBF3651B2056F28EBF859AE9#overview).

# Expanding Beyond the Undergraduate Curriculum

- **Nuclear physics**
  - Basic nuclear models (liquid drop, shell model and collective model), decay modes of radioactive nuclides ($α, β^+, β^−, γ$) and cross-section calculations of nuclear reactions.
  - [*Martin*](https://www.wiley.com/en-us/Nuclear+and+Particle+Physics%3A+An+Introduction%2C+3rd+Edition-p-9781119344612) and [*Krane*](https://www.wiley.com/en-us/Introductory+Nuclear+Physics%2C+3rd+Edition-p-9780471805533) are good starting points. [*Tina Potter’s slides*](https://www.hep.phy.cam.ac.uk/~chpotter/particleandnuclearphysics/mainpage.html) provide clear explanations and useful insights. For more details, refer to [*Blatt & Weisskopf*](https://link.springer.com/book/10.1007/978-1-4612-9959-2) for formal scattering theory.

- **Radiation physics**
  - Electron, photon, neutron interaction with matter. Concepts of KERMA, LET, stopping power, and dose. 
  - [*Turner*](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527616978) and [*Hooshang Nikjoo*](https://www.routledge.com/Interaction-of-Radiation-with-Matter/Nikjoo-Uehara-Emfietzoglou/p/book/9780367866020?srsltid=AfmBOor8xnXQC1WBWkicRN74gtG5SBA1yQae0BHI2zQaCsMWPPs2T-Ny) are helpful, refer to [*Podgorsak*](https://link.springer.com/book/10.1007/978-3-319-25382-4) and [*Podgorsak*](https://link.springer.com/book/10.1007/978-3-642-20186-8) for details.

- **Detection of radiation**
  - Principles of radiation detection, including gas-filled detectors, scintillators, and semiconductor detectors. Concepts like energy resolution, efficiency, dead time, and statistical uncertainty are crucial. Pulse processing and spectroscopy methods are also important for practical applications.
  - [*Knoll*](https://www.wiley.com/en-ae/Radiation+Detection+and+Measurement%2C+4th+Edition-p-9780470131480) is the standard reference.

- **Physics of radiotherapy**
  - Intensity-Modulated Radiation Therapy (IMRT), Volumetric Modulated Arc Therapy (VMAT), Image-Guided Radiation Therapy (IGRT), Stereotactic Body Radiation Therapy (SBRT), Boron Neutron Capture Therapy (BNCT), Proton Therapy, and Heavy Ion Therapy.
  - [*The Physics of Radiotherapy X-Rays and Electrons 3rd Edition*](https://medicalphysics.org/SimpleCMS.php?content=bookpage.php&isbn=9781951134105) and [*Khan’s The Physics of Radiation Therapy*](https://shop.lww.com/Khan-s-The-Physics-of-Radiation-Therapy/p/9781496397522?srsltid=AfmBOopw7KJsy68Iq6t5fNmViGW7WDQIXC6WdX8PdLDcxhLL__zHAxzC) provide a comprehensive overview.
  - AAPM Task Group reports serve as essential clinical references.

- **Physics of medical imaging**
  - Computed Tomography (CT), Magnetic Resonance Imaging (MRI), Positron Emission Tomography-Computed Tomography (PET-CT), and related imaging modalities.

- **Radiobiology and radiation protection**
  - Linear-Quadratic (LQ) model, bystander effects, ALARA principle and shielding calculations.
  - [*Radiobiology for the Radiologist 8th Edition*](https://shop.lww.com/Radiobiology-for-the-Radiologist/p/9781496335418?srsltid=AfmBOoo02iTJHtt_TgiT5JeADx5hU9Ajv1sa-huxtqe2FC83wHVL05ui) is the standard reference.

# Notes and Summaries
- **Summary of Nuclear physics:**  [PDF](https://louis-qiuyulu.github.io/summary of NP.pdf) 
- **Summary of Radiation physics:**  [PDF](https://louis-qiuyulu.github.io/CheatSheet-RP.pdf)  
- **Summary of Electrodynamics:**  [PDF](https://louis-qiuyulu.github.io/CheatSheet-EM.pdf)

---

## License  
These notes are licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).  

[![CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
