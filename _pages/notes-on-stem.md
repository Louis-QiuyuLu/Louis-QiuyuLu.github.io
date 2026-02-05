---
permalink: /notes-on-stem/
title: "Notes on STEM"
excerpt: "This page contains notes related to Science, Technology, Engineering, and Mathematics (STEM)."
author_profile: false
---

<span class='anchor' id='notes-on-stem'></span>

This page attempts to provide general guidance for undergraduate students in physics, biomedical engineering, or related STEM fields who are interested in medical physics.

The mathematical and physical foundations relevant to medical physics overlap only partially with those of a typical physics undergraduate curriculum. The field itself is broad, ranging from radiation physics and nuclear reactions to imaging and signal processing. Depending on one’s interests, different areas naturally become more prominent: for example, nuclear physics and dosimetry play a central role in radiation-focused paths, while image processing and mathematical tools (such as compressed sensing in MRI reconstruction) are crucial for imaging-oriented work. From what I have observed—and also from my own limited experience—it seems helpful to keep a wide perspective early on, while still building solid problem-solving habits.

As Landau once advised:

> “As to your question concerning the study of theoretical physics, I can state only that it is necessary to learn **ALL** its main branches, and the sequence of study is dictated by their mutual relationship. As a method of study, I can only emphasize that you must perform all the calculations by yourself, and must not leave it to the authors of the books you have read.”  
> – *L. D. Landau, cited in E. M. Lifshitz, Am. J. Phys. 45, 415 (1977); doi: 10.1119/1.10828*

Nowadays one might add that you should also not leave it to ChatGPT or DeepSeek. Feynman similarly emphasized the interconnectedness of different fields:

> “We make no apologies for making these excursions into other fields, because the separation of fields, as we have emphasized, is merely a human convenience, and an unnatural thing. Nature is not interested in our separations, and many of the interesting phenomena bridge the gaps between fields.”  
> – *R. P. Feynman, The Feynman Lectures on Physics, Vol. I, Ch. 35*

Just as Zhuangzi tells the story of opening the seven orifices from Chaos ([Hun-Dun](https://en.wikipedia.org/wiki/Hundun)), the natural world is inherently unified. Physics, as a description of nature, reflects this wholeness and cannot be fully understood if artificially fragmented into separate subjects.

Faced with a discipline as vast and historically layered as medical physics, it is natural to feel overwhelmed—like seeing only individual trees without perceiving the forest. In my own learning, I found that progress often resembles Emergentism more than strict Reductionism: through enough examples, calculations, and physical pictures, a larger structure begins to emerge. Occasionally this process even brings what I like to call a personal [**Aura**](https://en.wikipedia.org/wiki/The_Work_of_Art_in_the_Age_of_Mechanical_Reproduction)—a fleeting glimpse of the order underlying nature, revealed through thought and calculation.

The outline of theoretical foundations that follows is therefore only a personal sketch, shaped by my own biases and experiences. It is intended as a tentative guide, something that readers may adapt, expand, or even challenge in their own learning journey. My hope is that it offers a starting point for exploring the physics underlying medical and engineering applications, without claiming to be definitive or exhaustive.

# Fundamental Commonly Covered in Undergraduate

- **Mathematical methods in physics**
  - ODEs and PDEs, Contour Integral, Green’s functions, and variational methods. Special functions like Legendre, Bessel, and spherical harmonics appear often. Group theory and Lie algebra are also helpful for advanced theory.
  - [*Hassani*](https://link.springer.com/book/10.1007/978-3-319-01195-0) is good for a general overview and advanced details, the explanations are clear, and the solved examples make it easier to see how the methods are applied.

- **Computational methods**
  - Monte Carlo simulation ([Geant4](https://geant4.web.cern.ch/), [FLUKA](http://www.fluka.org/fluka.php?)) for radiation transport, finite element methods(COMSOL, ANSYS) for solving EM field problems, and numerical techniques for dose calculation.
  - For practical applications, open-source toolkits, examples and software manuals are often useful.

- **Quantum mechanics**

  <p align="center">
    <img src="../images/QM_DND.jpg" alt="DND Alignment of QM texts." width="50%">
  </p>

  - Knowledge until second quantization (so-called advanced quantum mechanics) is enough. Most problems in medical physics deal with atomic-level fine-structure effects, such as spin-orbit coupling and relativistic corrections. QFT is unnecessary unless calculating exact reaction cross-sections, secondary electron production in radiotherapy or higher-order corrections in positron annihilation processes.
  - [*Griffiths*](https://www.cambridge.org/highereducation/books/introduction-to-quantum-mechanics/990799CA07A83FC5312402AF6860311E#overview), [*Sakurai*](https://www.cambridge.org/highereducation/books/modern-quantum-mechanics/DF43277E8AEDF83CC12EA62887C277DC#overview) are both accessible for beginners. Griffiths is very readable and focuses on building intuition through clear examples, making it easier to grasp the fundamental concepts. Sakurai is a bit more formal and abstract but provides a solid foundation for understanding modern quantum mechanics. Refer to [*Cohen-Tannoudji*](https://www.wiley.com/en-us/Quantum+Mechanics%2C+Volume+1%3A+Basic+Concepts%2C+Tools%2C+and+Applications%2C+2nd+Edition-p-9783527822713) for details, it goes deeper into both the formalism and applications, and the worked examples are very helpful if you want to really see the methods in action.

- **Electrodynamics**
  - Calculation of EM fields, relativistically charged particle dynamics, wave propagation in biological tissues and detectors.
  - Begin with [*Griffiths*](https://www.cambridge.org/highereducation/books/introduction-to-electrodynamics/3AB220820DBB628E5A43D52C4B011ED4#overview), which is very readable and provides clear explanations of fundamental concepts with plenty of examples. It’s ideal for building intuition and getting comfortable with vector calculus in physics. Advance to [*Jackson*](https://www.wiley.com/en-au/Classical+Electrodynamics%2C+3rd+Edition-p-9780471309321) and [*Zangwill*](https://www.cambridge.org/highereducation/books/modern-electrodynamics/E5448C70CBF3651B2056F28EBF859AE9#overview). Jackson as standard graduate textbook of electrodynamics is more formal and mathematically rigorous, excellent for developing a deep theoretical understanding and tackling challenging problems; however, its Chapter 13 on collisions between charged particles, which relates to medical physics, is not very well structured and some calculations are not entirely rigorous. Zangwill offers a modern perspective, covering topics not included in Jackson, and its explanations are generally more approachable for self-study.

# Beyond the Undergraduate

- **Nuclear physics**
  - Basic nuclear models (liquid drop, shell model and collective model), decay modes of radioactive nuclides ($α, β^+, β^−, γ$) and cross-section calculations of nuclear reactions.
  - [*Martin*](https://www.wiley.com/en-us/Nuclear+and+Particle+Physics%3A+An+Introduction%2C+3rd+Edition-p-9781119344612) and [*Krane*](https://www.wiley.com/en-us/Introductory+Nuclear+Physics%2C+3rd+Edition-p-9780471805533) are both solid starting points. Martin is quite accessible, giving clear explanations and covering a broad range of topics, while Krane provides a slightly more detailed treatment with helpful examples for understanding nuclear structure and reactions. [*Tina Potter’s slides*](https://www.hep.phy.cam.ac.uk/~chpotter/particleandnuclearphysics/mainpage.html) are excellent for quick overviews and intuitive explanations; For a more formal and in-depth treatment of scattering theory, [*Blatt & Weisskopf*](https://link.springer.com/book/10.1007/978-1-4612-9959-2) first published in 1952 remains a classic reference, though it’s more mathematically heavy and best approached after getting comfortable with the basics.

- **Radiation physics**
  - Photon, neutron and charged particle interaction with matter.
  - [*Turner*](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527616978) and [*Hooshang Nikjoo*](https://www.routledge.com/Interaction-of-Radiation-with-Matter/Nikjoo-Uehara-Emfietzoglou/p/book/9780367866020?srsltid=AfmBOor8xnXQC1WBWkicRN74gtG5SBA1yQae0BHI2zQaCsMWPPs2T-Ny) are quite readable and gives a good introduction to the principles. [*Radiation Physics for Medical Physicists*](https://link.springer.com/book/10.1007/978-3-319-25382-4) is very useful, offering practical context and examples that connect the theory to clinical practice.

- **Detection of radiation**
  - Principles of radiation detection, including gas-filled detectors, scintillators, and semiconductor detectors. Concepts like energy resolution, efficiency, dead time, and statistical uncertainty are crucial. Pulse processing and spectroscopy methods are also important for practical applications.
  - [*Knoll*](https://www.wiley.com/en-ae/Radiation+Detection+and+Measurement%2C+4th+Edition-p-9780470131480) is a classic and very comprehensive; it’s detailed and mathematically rigorous, making it an excellent reference once you are comfortable with the basics. [*Attix*](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527617135) focuses more on dosimetry and practical aspects, and is easier to read for beginners. [*Fundamentals of Ionizing Radiation Dosimetry*](https://www.wiley.com/en-us/Fundamentals+of+Ionizing+Radiation+Dosimetry-p-9783527409211) is helpful for connecting detector physics with dosimetric calculations, providing a bridge between theory and medical applications.

- **Physics of radiotherapy**
  - Intensity-Modulated Radiation Therapy (IMRT), Volumetric Modulated Arc Therapy (VMAT), Image-Guided Radiation Therapy (IGRT), Stereotactic Body Radiation Therapy (SBRT), Boron Neutron Capture Therapy (BNCT), Proton Therapy, and Heavy Ion Therapy.
  - [*The Physics of Radiotherapy X-Rays and Electrons 3rd Edition*](https://medicalphysics.org/SimpleCMS.php?content=bookpage.php&isbn=9781951134105) and [*Khan’s The Physics of Radiation Therapy*](https://shop.lww.com/Khan-s-The-Physics-of-Radiation-Therapy/p/9781496397522?srsltid=AfmBOopw7KJsy68Iq6t5fNmViGW7WDQIXC6WdX8PdLDcxhLL__zHAxzC) provide a comprehensive overview.
  - AAPM Task Group reports and ICRU reports serve as essential clinical references.

- **Physics of medical imaging**
  - Computed Tomography (CT), Magnetic Resonance Imaging (MRI), Positron Emission Tomography-Computed Tomography (PET-CT), Ultrasound Imaging and other related imaging modalities.
  - [*The Essential Physics of Medical Imaging, 3rd Edition*](https://pubmed.ncbi.nlm.nih.gov/28524933/), [*Fundamental Mathematics and Physics of Medical Imaging*](https://doi.org/10.1201/9781315368214) and [*Medical Imaging Physics, 4th Edition*](https://www.wiley.com/en-us/Medical+Imaging+Physics%2C+4th+Edition-p-9780471461135).

- **Radiobiology and radiation protection**
  - Covers the fundamentals of radiobiology, including the Linear-Quadratic (LQ) model for cell survival, bystander effects, and the abscopal effect. Radiation protection topics include the ALARA principle, dose limits, and shielding calculations.
  - [*Radiobiology for the Radiologist 8th Edition*](https://shop.lww.com/Radiobiology-for-the-Radiologist/p/9781496335418?srsltid=AfmBOoo02iTJHtt_TgiT5JeADx5hU9Ajv1sa-huxtqe2FC83wHVL05ui).

# Cheatsheets, Notes and Summaries (Feedback and typo corrections are welcome!)
- **Electromagnetism:**  [PDF](https://louis-qiuyulu.github.io/CheatSheet-EM.pdf)
- **Nuclear physics:**  [PDF](https://louis-qiuyulu.github.io/summary-of-NP.pdf) 
- **Radiation physics:**  [PDF](https://louis-qiuyulu.github.io/CheatSheet-RP.pdf)
- **Medical imaging:**  [PDF](https://louis-qiuyulu.github.io/summary-of-MI.pdf)
- **Physics of radiotherapy:**  [PDF](https://louis-qiuyulu.github.io/summary-of-RT.pdf)

---

## License  
These notes are licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).  

[![CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
