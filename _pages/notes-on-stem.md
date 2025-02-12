---
permalink: /notes-on-stem/
title: "Notes on STEM"
excerpt: "This page contains notes related to Science, Technology, Engineering, and Mathematics (STEM)."
author_profile: false
---

<span class='anchor' id='notes-on-stem'></span>

To transition into medical physics with a foundational background in science or engineering at the undergraduate level, one should have a solid understanding of the following STEM subjects:

# Covered or at least mentioned in standard undergraduate physics

- **Mathematical methods in physics**
  - Partial differential equations, Green’s functions, and variational methods. Special functions like Legendre, Bessel, and spherical harmonics appear often but usually in pre-tabulated or numerically evaluated forms.
  - [Hassani](https://link.springer.com/book/10.1007/978-3-319-01195-0) is good for a general overview and advanced details. Numerical methods book are more practical.

- **Computational methods**
  - Monte Carlo simulation (e.g., [Geant4](https://geant4.web.cern.ch/), [FLUKA](http://www.fluka.org/fluka.php?)) for radiation transport, finite element methods for solving EM field problems, and numerical techniques for dose calculation (e.g., pencil beam, Monte Carlo dose engines).
  - For practical applications, open-source toolkits and software manuals are often more useful than standard textbooks.

- **Quantum mechanics**
  - Knowledge until second quantization (so-called advanced quantum mechanics) is enough. Most problems in MP deal with things at the fine structure of the atomic level like spin-orbit coupling and relativistic corrections. QFT is not necessary unless you have to calculate exact reaction cross-sections in nuclear physics.
  - [Griffiths](https://www.cambridge.org/highereducation/books/introduction-to-quantum-mechanics/990799CA07A83FC5312402AF6860311E#overview), [Sakurai](https://www.cambridge.org/highereducation/books/modern-quantum-mechanics/DF43277E8AEDF83CC12EA62887C277DC#overview) are fine for beginners, refer to [Cohen-Tannoudji](https://www.wiley.com/en-us/Quantum+Mechanics%2C+Volume+1%3A+Basic+Concepts%2C+Tools%2C+and+Applications%2C+2nd+Edition-p-9783527822713) for details.

- **Electrodynamics**
  - Calculation of EM fields (most problems do not have analytic solutions, involving complex analysis and weird special functions, requiring finite element methods) and relativistically charged particle dynamics. QED is still unnecessary but no harm if you are really interested in the calculation of Feynman diagrams.
  - Begin with [Griffiths](https://www.cambridge.org/highereducation/books/introduction-to-electrodynamics/3AB220820DBB628E5A43D52C4B011ED4#overview), advance to [Jackson](https://www.wiley.com/en-au/Classical+Electrodynamics%2C+3rd+Edition-p-9780471309321) and [Zangwill](https://www.cambridge.org/highereducation/books/modern-electrodynamics/E5448C70CBF3651B2056F28EBF859AE9#overview).

- **Nuclear physics**
  - Basic nuclear models (liquid drop, shell model), nuclear reactions, decay processes, and detector principles.
  - [Martin](https://www.wiley.com/en-us/Nuclear+and+Particle+Physics%3A+An+Introduction%2C+3rd+Edition-p-9781119344612) and [Krane](https://www.wiley.com/en-us/Introductory+Nuclear+Physics%2C+3rd+Edition-p-9780471805533) are good starting points. [Tina Potter’s slides](https://www.hep.phy.cam.ac.uk/~chpotter/particleandnuclearphysics/mainpage.html) provide clear explanations and useful insights. For more details, refer to [Blatt & Weisskopf](https://link.springer.com/book/10.1007/978-1-4612-9959-2) for formal scattering theory.

# New things perhaps

- **Radiation physics**
  - Electron, photon, neutron interaction with matter. Concepts of KERMA, LET, stopping power, and dose. 
  - [Turner](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527616978) and [Hooshang Nikjoo, Shuzo Uehara, Dimitris Emfietzoglou](https://www.routledge.com/Interaction-of-Radiation-with-Matter/Nikjoo-Uehara-Emfietzoglou/p/book/9780367866020?srsltid=AfmBOor8xnXQC1WBWkicRN74gtG5SBA1yQae0BHI2zQaCsMWPPs2T-Ny) are helpful, refer to [Podgorsak](https://link.springer.com/book/10.1007/978-3-319-25382-4) and [Podgorsak](https://link.springer.com/book/10.1007/978-3-642-20186-8) for details.

- **Detection of radiation**
  - Principles of radiation detection, including gas-filled detectors, scintillators, and semiconductor detectors. Concepts like energy resolution, efficiency, dead time, and statistical uncertainty are crucial. Pulse processing and spectroscopy methods are also important for practical applications.
  - [Knoll](https://www.wiley.com/en-ae/Radiation+Detection+and+Measurement%2C+4th+Edition-p-9780470131480) is the standard reference.

- **Physics of radiotherapy**
  - IMRT, VMAT, IGRT, etc.
  - [Metcalfe](https://medicalphysics.org/SimpleCMS.php?content=bookpage.php&isbn=9781951134105) is very detailed.

- **Physics of medical imaging**
  - CT, MRI, PET-CT, etc.

- **Radiobiology and radiation protection**
  - tbc.

# Not so helpful notes and summarys
- **Summary of Radiation Physics:**  [PDF](https://louis-qiuyulu.github.io/CheatSheet-RP.pdf)  
- **Summary of Electrodynamics:**  [PDF](https://louis-qiuyulu.github.io/CheatSheet-EM.pdf)  

---

## License  
These notes are licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).  

[![CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
