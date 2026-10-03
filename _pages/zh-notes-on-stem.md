---
permalink: /zh/notes-on-stem/
title: "理工笔记"
excerpt: "与科学、技术、工程与数学（STEM）相关的笔记。"
author_profile: false
lang: zh
ref: notes-on-stem
---

<span class='anchor' id='notes-on-stem'></span>

本页试图为对医学物理感兴趣的物理、生物医学工程及相关 STEM 专业本科生提供一般性指引。

与医学物理相关的数学与物理基础，与典型物理学本科课程仅部分重合。这一领域本身非常广阔，从辐射物理、核反应到成像与信号处理皆有涉及。兴趣不同，侧重点也会不同：例如，辐射相关路径中核物理与剂量学居核心地位；而成像方向则更依赖图像处理与数学工具（如 MRI 重建中的压缩感知）。就我所见——以及我自身有限的经验——早期保持较宽的视野，同时养成扎实的解题习惯，会很有帮助。

正如朗道曾经建议的：

> “至于你关于理论物理学习的问题，我只能说：必须学习其**所有**主要分支，学习顺序则由其相互关系决定。至于方法，我只能强调：一切计算都必须亲自完成，而不能交给你所读书籍的作者。”  
> – *L. D. Landau，引自 E. M. Lifshitz, Am. J. Phys. 45, 415 (1977); doi: 10.1119/1.10828*

如今或许还要补充：也不要把计算交给 ChatGPT 或 DeepSeek。费曼同样强调不同领域之间的内在联系：

> “我们并不为这些跨领域的旁逸斜出而道歉，因为正如我们所强调的，学科划分只是人类的便利，而非自然之事。自然并不关心我们的分界，许多有趣的现象恰恰跨越了这些鸿沟。”  
> – *R. P. Feynman, The Feynman Lectures on Physics, Vol. I, Ch. 35*

正如庄子所讲开凿混沌七窍的故事（[浑沌](https://en.wikipedia.org/wiki/Hundun)），自然界本身是统一的。物理学作为对自然的描述，也反映这种整体性；若被人为割裂成彼此孤立的科目，便难以真正理解。

面对医学物理这样一门广袤且历史层层叠叠的学科，感到不知所措是自然的——仿佛只见树木而不见森林。在我自己的学习中，进展往往更像涌现论（Emergentism）而非严格还原论：通过足够多的例子、计算与物理图像，更大的结构会逐渐显现。偶尔，这一过程还会带来我喜欢称作个人 [**Aura**](https://en.wikipedia.org/wiki/The_Work_of_Art_in_the_Age_of_Mechanical_Reproduction) 的瞬间——经由思考与计算，短暂瞥见自然底层秩序的微光。

因此，下文关于理论基础的提纲只是个人草图，受我自身偏见与经验塑造。它意在作为试探性指南，读者可以在自己的学习旅程中加以改编、扩展乃至质疑。我希望它能为探索医学与工程应用背后的物理提供一个起点，而不自称权威或穷尽。

# 本科阶段常见基础

- **物理中的数学方法**
  - 常微分方程与偏微分方程、复变围道积分、格林函数与变分法。勒让德函数、贝塞尔函数与球谐函数等特殊函数经常出现。群论与李代数对进阶理论也很有帮助。
  - [*Hassani*](https://link.springer.com/book/10.1007/978-3-319-01195-0) 适合总览与深入细节，讲解清晰，例题有助于看清方法如何应用。

- **计算方法**
  - 用于辐射输运的蒙特卡罗模拟（[Geant4](https://geant4.web.cern.ch/)：通用粒子输运与复杂探测器从头建模；[FLUKA](http://www.fluka.org/fluka.php?)：高能物理、设施屏蔽与辐射防护；[TOPAS](https://www.topasmc.org/)：参数驱动的放疗建模；[FRED](https://www.fred-mc.org/Manual_3.76/index.html)：带电粒子治疗中的 GPU 加速束流计算与质量保证），用于求解电磁场问题的有限元方法（COMSOL、ANSYS），以及剂量计算的数值技术。
  - 实际应用中，开源工具包、示例与软件手册往往很有用。

- **量子力学**

  <p align="center">
    <img src="{{ site.baseurl }}/images/QM_DND.jpg" alt="量子力学教材对照。" width="50%">
  </p>

  - 学到二次量子化（所谓高等量子力学）通常足够。医学物理中的多数问题涉及原子尺度精细结构效应，如自旋—轨道耦合与相对论修正。除非计算精确反应截面、放疗中的次级电子产生，或正电子湮灭过程中的高阶修正，否则不必深入量子场论。
  - [*Griffiths*](https://www.cambridge.org/highereducation/books/introduction-to-quantum-mechanics/990799CA07A83FC5312402AF6860311E#overview) 与 [*Sakurai*](https://www.cambridge.org/highereducation/books/modern-quantum-mechanics/DF43277E8AEDF83CC12EA62887C277DC#overview) 对初学者都较易入手。Griffiths 可读性强，善于通过清晰例子建立直觉；Sakurai 更形式、更抽象，但为理解现代量子力学提供了坚实基础。细节可参考 [*Cohen-Tannoudji*](https://www.wiley.com/en-us/Quantum+Mechanics%2C+Volume+1%3A+Basic+Concepts%2C+Tools%2C+and+Applications%2C+2nd+Edition-p-9783527822713)，它对形式体系与应用都更深入，例题对真正掌握方法很有帮助。

- **电动力学**
  - 电磁场计算、相对论带电粒子动力学、电磁波在生物组织与探测器中的传播。
  - 可从 [*Griffiths*](https://www.cambridge.org/highereducation/books/introduction-to-electrodynamics/3AB220820DBB628E5A43D52C4B011ED4#overview) 开始，它可读性强，对基本概念有清晰解释与大量例子，适合建立直觉并熟悉物理中的矢量微积分。随后可进阶到 [*Jackson*](https://www.wiley.com/en-au/Classical+Electrodynamics%2C+3rd+Edition-p-9780471309321) 与 [*Zangwill*](https://www.cambridge.org/highereducation/books/modern-electrodynamics/E5448C70CBF3651B2056F28EBF859AE9#overview)。Jackson 作为研究生标准教材更形式、更数学严格，有助于深化理论理解并挑战难题；但其第 13 章关于带电粒子碰撞（与医学物理相关）结构不够理想，部分计算也不尽严谨。Zangwill 提供更现代的视角，涵盖 Jackson 未涉及的内容，解释通常更适合自学。

# 超越本科

- **核物理**
  - 基本核模型（液滴模型、壳模型与集体模型），放射性核素衰变模式（$α, β^+, β^−, γ$），以及核反应截面计算。
  - [*Martin*](https://www.wiley.com/en-us/Nuclear+and+Particle+Physics%3A+An+Introduction%2C+3rd+Edition-p-9781119344612) 与 [*Krane*](https://www.wiley.com/en-us/Introductory+Nuclear+Physics%2C+3rd+Edition-p-9780471805533) 都是扎实的入门选择。Martin 较为易读，覆盖面广；Krane 稍更细致，对理解核结构与反应有帮助的例子。[*Tina Potter 的讲义*](https://www.hep.phy.cam.ac.uk/~chpotter/particleandnuclearphysics/mainpage.html) 适合快速总览与直觉理解；对散射理论更形式、更深入的处理，1952 年初版的 [*Blatt & Weisskopf*](https://link.springer.com/book/10.1007/978-1-4612-9959-2) 仍是经典参考，但数学较重，最好在熟悉基础后再读。

- **辐射物理**
  - 光子、中子与带电粒子与物质的相互作用。
  - [*Turner*](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527616978) 与 [*Hooshang Nikjoo*](https://www.routledge.com/Interaction-of-Radiation-with-Matter/Nikjoo-Uehara-Emfietzoglou/p/book/9780367866020?srsltid=AfmBOor8xnXQC1WBWkicRN74gtG5SBA1yQae0BHI2zQaCsMWPPs2T-Ny) 可读性较好，是原理入门的好选择。[*Radiation Physics for Medical Physicists*](https://link.springer.com/book/10.1007/978-3-319-25382-4) 非常实用，提供将理论与临床实践相连的情境与例子。

- **辐射探测**
  - 辐射探测原理，包括气体探测器、闪烁体与半导体探测器。能量分辨率、效率、死时间与统计不确定度等概念至关重要。脉冲处理与谱学方法对实际应用也很重要。
  - [*Knoll*](https://www.wiley.com/en-ae/Radiation+Detection+and+Measurement%2C+4th+Edition-p-9780470131480) 是经典且全面的参考，细节充分、数学严格，适合在掌握基础后深入查阅。[*Attix*](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527617135) 更侧重剂量学与实践方面，对初学者更易读。[*Fundamentals of Ionizing Radiation Dosimetry*](https://www.wiley.com/en-us/Fundamentals+of+Ionizing+Radiation+Dosimetry-p-9783527409211) 有助于把探测器物理与剂量学计算联系起来，在理论与医学应用之间架桥。

- **放射治疗物理**
  - 调强放射治疗（IMRT）、容积调强弧形治疗（VMAT）、图像引导放射治疗（IGRT）、立体定向体部放射治疗（SBRT）、硼中子俘获治疗（BNCT）、质子治疗与重离子治疗。
  - [*The Physics of Radiotherapy X-Rays and Electrons 3rd Edition*](https://medicalphysics.org/SimpleCMS.php?content=bookpage.php&isbn=9781951134105) 与 [*Khan’s The Physics of Radiation Therapy*](https://shop.lww.com/Khan-s-The-Physics-of-Radiation-Therapy/p/9781496397522?srsltid=AfmBOopw7KJsy68Iq6t5fNmViGW7WDQIXC6WdX8PdLDcxhLL__zHAxzC) 提供全面概览。
  - AAPM Task Group 报告与 ICRU 报告是重要的临床参考。

- **医学影像物理**
  - 计算机断层成像（CT）、磁共振成像（MRI）、正电子发射断层—计算机断层成像（PET-CT）、超声成像及其他相关成像模态。
  - [*The Essential Physics of Medical Imaging, 3rd Edition*](https://pubmed.ncbi.nlm.nih.gov/28524933/)、[*Fundamental Mathematics and Physics of Medical Imaging*](https://doi.org/10.1201/9781315368214) 与 [*Medical Imaging Physics, 4th Edition*](https://www.wiley.com/en-us/Medical+Imaging+Physics%2C+4th+Edition-p-9780471461135)。

- **放射生物学与辐射防护**
  - 涵盖放射生物学基础，包括细胞存活的线性—二次（LQ）模型、旁观者效应与远隔效应（abscopal effect）。辐射防护主题包括 ALARA 原则、剂量限值与屏蔽计算。
  - [*Radiobiology for the Radiologist 8th Edition*](https://shop.lww.com/Radiobiology-for-the-Radiologist/p/9781496335418?srsltid=AfmBOoo02iTJHtt_TgiT5JeADx5hU9Ajv1sa-huxtqe2FC83wHVL05ui)。

# 速查表、笔记与摘要（欢迎反馈与勘误！）
- **电磁学：**  [PDF](https://louis-qiuyulu.github.io/CheatSheet-EM.pdf)
- **核物理：**  [PDF](https://louis-qiuyulu.github.io/summary-of-NP.pdf) 
- **辐射物理：**  [PDF](https://louis-qiuyulu.github.io/CheatSheet-RP.pdf)
- **医学影像：**  [PDF](https://louis-qiuyulu.github.io/summary-of-MI.pdf)
- **放射治疗物理：**  [PDF](https://louis-qiuyulu.github.io/summary-of-RT.pdf)
- **辐射防护与放射生物学：**  [PDF](https://louis-qiuyulu.github.io/summary_of_RB.pdf)

---

## 许可协议  
本笔记采用 [知识共享署名—非商业性使用—相同方式共享 4.0 国际许可协议](https://creativecommons.org/licenses/by-nc-sa/4.0/) 授权。  

[![CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
