---
permalink: /zh/notes-on-stem/
title: "理工笔记"
excerpt: "与科学、技术、工程与数学（STEM）相关的笔记。"
author_profile: false
lang: zh
ref: notes-on-stem
---

<span class='anchor' id='notes-on-stem'></span>

本页旨在为对医学物理感兴趣的物理、生物医学工程及相关 STEM 专业本科生，提供一份通用的参考指引。

医学物理所需的数理基础，与物理系本科课程仅有部分重合。这个领域跨度极大，涵盖辐射物理、核反应、医学成像乃至信号处理。方向不同，侧重也各有千秋：走辐射物理路线，核物理与剂量学是核心；偏向成像方向，则更依赖图像处理与数学工具（如 MRI 重建中的压缩感知）。依我浅见，加上自己有限的学习体会，在起步阶段拓宽视野、多做推导并养成扎实的解题习惯，往往大有裨益。

正如朗道曾告诫年轻学生的：

> “至于你关于理论物理学习的问题，我只能说：必须学完理论物理的**所有**主要分支，学习顺序则取决于它们之间的内在联系。至于方法，我必须强调：所有计算都得亲手推导，切不可留给你所读书籍的作者。”  
> – *L. D. Landau，引自 E. M. Lifshitz, Am. J. Phys. 45, 415 (1977); doi: 10.1119/1.10828*

放在当下，或许还得补上一句：也不要把推导全部推给各类大语言模型。费曼同样十分看重学科之间的浑然一体：

> “我们无需为跨领域的旁逸斜出而致歉。正如我们常说的，学科划分不过是人为图个方便，大自然本身并无界限。自然并不在乎我们划定的篱笆，许多耐人寻味的现象恰恰出现在学科的交界处。”  
> – *R. P. Feynman, The Feynman Lectures on Physics, Vol. I, Ch. 35*

正如庄子所述[浑沌](https://en.wikipedia.org/wiki/Hundun)凿七窍的故事，自然本是完整的统一体。物理学用以描摹自然，自当映照出这种整体性；若人为将其割裂为互不相干的条块，反倒难以得其精髓。

面对医学物理这门枝繁叶茂、沉淀深厚的学科，初学者容易有“只见树木、不见森林”的迷茫感。就我自身的体会而言，掌握这门学科的过程更贴近“涌现”，而非机械的还原：当你积累了足够多的推导、算例与物理图景，整体的脉络自然会水落石出。偶尔，这种推演还会带来所谓的灵光（[**Aura**](https://en.wikipedia.org/wiki/The_Work_of_Art_in_the_Age_of_Mechanical_Reproduction)）——在纸笔推导之间，得以一瞥自然底层运行律则的微光。

因此，下文整理的理论基础只是我个人的读书小结，难免带有些许个人偏好与经验局限。它仅作为抛砖引玉的参考，读者尽可在自己的求学途中取舍、补充甚至质疑。倘若它能为大家探索医学与工程背后的物理世界提供一个切入点，便达到了初衷。

# 本科基础课程

- **数学物理方法**
  - 常微分方程与偏微分方程、复变围道积分、格林函数与变分法。勒让德多项式、贝塞尔函数及球谐函数等特殊函数经常登场。进阶理论中，群论与李代数同样不可或缺。
  - [*Hassani*](https://link.springer.com/book/10.1007/978-3-319-01195-0) 兼顾宏观脉络与细部推演，叙述透彻，例题很适合用来摸清具体方法的运用。

- **计算物理与数值模拟**
  - 辐射输运蒙特卡罗模拟（[Geant4](https://geant4.web.cern.ch/)：通用粒子输运与复杂探测器建模；[FLUKA](http://www.fluka.org/fluka.php?)：高能物理、屏蔽设计与辐射防护；[TOPAS](https://www.topasmc.org/)：参数化放疗建模；[FRED](https://www.fred-mc.org/Manual_3.76/index.html)：用于带电粒子治疗的 GPU 束流加速计算与质控）、有限元方法求解电磁场（COMSOL、ANSYS），以及剂量计算的常用数值算法。
  - 实践中，熟读开源工具包、代码示例与官方手册往往能事半功倍。

- **量子力学**

  <p align="center">
    <img src="{{ site.baseurl }}/images/QM_DND.jpg" alt="量子力学教材对照。" width="50%">
  </p>

  - 学到二次量子化（高等量子力学阶段）一般已足够应对多数问题。医学物理主要关注自旋—轨道耦合、相对论修正等原子尺度的精细结构效应。除非要精确计算核反应截面、放疗中的次级电子产生，抑或正电子湮灭的高阶修正，否则通常无须深涉量子场论。
  - [*Griffiths*](https://www.cambridge.org/highereducation/books/introduction-to-quantum-mechanics/990799CA07A83FC5312402AF6860311E#overview) 与 [*Sakurai*](https://www.cambridge.org/highereducation/books/modern-quantum-mechanics/DF43277E8AEDF83CC12EA62887C277DC#overview) 都是极好的入门读物。Griffiths 读来通俗生动，善用直观算例构建图像；Sakurai 形式感更强、偏重抽象代数框架，能为现代量子理论打下坚实底子。若想深究推导细节，可参考 [*Cohen-Tannoudji*](https://www.wiley.com/en-us/Quantum+Mechanics%2C+Volume+1%3A+Basic+Concepts%2C+Tools%2C+and+Applications%2C+2nd+Edition-p-9783527822713)，其体系严整、应用广泛，书中的练习题非常锻炼实战功夫。

- **电动力学**
  - 电磁场解析、相对论带电粒子动力学、电磁波在生物组织与探测介质中的传播规律。
  - 可以从 [*Griffiths*](https://www.cambridge.org/highereducation/books/introduction-to-electrodynamics/3AB220820DBB628E5A43D52C4B011ED4#overview) 入手，文字流畅，概念剖析到位，且附带大量矢量微积分示例，极易上手并建立直觉。进阶阶段推荐 [*Jackson*](https://www.wiley.com/en-au/Classical+Electrodynamics%2C+3rd+Edition-p-9780471309321) 和 [*Zangwill*](https://www.cambridge.org/highereducation/books/modern-electrodynamics/E5448C70CBF3651B2056F28EBF859AE9#overview)。Jackson 作为经典的研究生教材，推导严谨、数学深度足，很适合磨炼硬核理论功底；但其第 13 章涉及带电粒子碰撞（与医学物理直接相关）的脉络略显晦涩，个别推算不够爽利。相比之下，Zangwill 视角更现代，补足了不少前书未谈及的内容，整体更利于自学。

# 专业与进阶方向

- **核物理**
  - 原子核基本模型（液滴模型、壳层模型与集体模型）、核素衰变模式（$α, β^+, β^−, γ$），以及核反应截面计算。
  - [*Martin*](https://www.wiley.com/en-us/Nuclear+and+Particle+Physics%3A+An+Introduction%2C+3rd+Edition-p-9781119344612) 与 [*Krane*](https://www.wiley.com/en-us/Introductory+Nuclear+Physics%2C+3rd+Edition-p-9780471805533) 皆为经典的入门教本。Martin 叙述浅白、知识面宽；Krane 剖析更细致，配有大量辅助理解核结构与核反应的实例。若想迅速搭建直观概念，不妨参阅 [*Tina Potter 讲义*](https://www.hep.phy.cam.ac.uk/~chpotter/particleandnuclearphysics/mainpage.html)；若想深究散射理论的形式体系，1952 年首版的 [*Blatt & Weisskopf*](https://link.springer.com/book/10.1007/978-1-4612-9959-2) 依然是权威专著，但其数学门槛较高，建议打牢基础后再作精读。

- **辐射物理**
  - 光子、中子及带电粒子与物质的相互作用。
  - [*Turner*](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527616978) 和 [*Hooshang Nikjoo*](https://www.routledge.com/Interaction-of-Radiation-with-Matter/Nikjoo-Uehara-Emfietzoglou/p/book/9780367866020?srsltid=AfmBOor8xnXQC1WBWkicRN74gtG5SBA1yQae0BHI2zQaCsMWPPs2T-Ny) 条理分明，通俗晓畅，是掌握相互作用机理的优质教材。[*Radiation Physics for Medical Physicists*](https://link.springer.com/book/10.1007/978-3-319-25382-4) 则重在实用，书中结合了大量临床场景与算例，方便将理论直接对接医院实践。

- **辐射探测**
  - 辐射探测机理，囊括气体探测器、闪烁体与半导体探测器。重点掌握能量分辨率、探测效率、死时间及统计涨落等核心概念，同时结合实际工程，熟悉脉冲成形与能谱分析方法。
  - [*Knoll*](https://www.wiley.com/en-ae/Radiation+Detection+and+Measurement%2C+4th+Edition-p-9780470131480) 堪称案头必备宝典，内容详尽、推演扎实，适合夯实基础后当作工具书随查随用。[*Attix*](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527617135) 偏重实用剂量学，读起来更轻松。[*Fundamentals of Ionizing Radiation Dosimetry*](https://www.wiley.com/en-us/Fundamentals+of+Ionizing+Radiation+Dosimetry-p-9783527409211) 则把探测器物理同剂量算法紧密编织在一起，架起了从基础物理通往临床应用的桥梁。

- **放射治疗物理**
  - 调强放疗（IMRT）、容积旋转调强放疗（VMAT）、图像引导放疗（IGRT）、立体定向体部放疗（SBRT）、硼中子俘获治疗（BNCT）、质子与重离子治疗。
  - [*The Physics of Radiotherapy X-Rays and Electrons (3rd Edition)*](https://medicalphysics.org/SimpleCMS.php?content=bookpage.php&isbn=9781951134105) 与 [*Khan’s The Physics of Radiation Therapy*](https://shop.lww.com/Khan-s-The-Physics-of-Radiation-Therapy/p/9781496397522?srsltid=AfmBOopw7KJsy68Iq6t5fNmViGW7WDQIXC6WdX8PdLDcxhLL__zHAxzC) 是临床放疗物理的必备全景参考书。
  - 此外，AAPM Task Group 与 ICRU 系列报告是开展临床质控与剂量计算的行业准则，务必经常查阅。

- **医学影像物理**
  - 计算机断层成像（CT）、磁共振成像（MRI）、正电子发射计算机断层显像（PET-CT）、超声成像及各类多模态影像。
  - 核心读物推荐：[*The Essential Physics of Medical Imaging (3rd Edition)*](https://pubmed.ncbi.nlm.nih.gov/28524933/)、[*Fundamental Mathematics and Physics of Medical Imaging*](https://doi.org/10.1201/9781315368214) 以及 [*Medical Imaging Physics (4th Edition)*](https://www.wiley.com/en-us/Medical+Imaging+Physics%2C+4th+Edition-p-9780471461135)。

- **放射生物学与辐射防护**
  - 放射生物学核心内容包含细胞存活线性二次模型（LQ 模型）、旁效应（bystander effect）与远隔效应（abscopal effect）。辐射防护则围绕 ALARA 原则、剂量限值与屏蔽厚度设计展开。
  - 首选参考教材为 [*Radiobiology for the Radiologist (8th Edition)*](https://shop.lww.com/Radiobiology-for-the-Radiologist/p/9781496335418?srsltid=AfmBOoo02iTJHtt_TgiT5JeADx5hU9Ajv1sa-huxtqe2FC83wHVL05ui)。

# 速查手册、笔记与讲义（恳请批评斧正！）
- **电磁学：** [PDF](https://louis-qiuyulu.github.io/CheatSheet-EM.pdf)
- **核物理：** [PDF](https://louis-qiuyulu.github.io/summary-of-NP.pdf) 
- **辐射物理：** [PDF](https://louis-qiuyulu.github.io/CheatSheet-RP.pdf)
- **医学影像：** [PDF](https://louis-qiuyulu.github.io/summary-of-MI.pdf)
- **放射治疗物理：** [PDF](https://louis-qiuyulu.github.io/summary-of-RT.pdf)
- **辐射防护与放射生物学：** [PDF](https://louis-qiuyulu.github.io/summary_of_RB.pdf)

---

## 许可协议  
本页面笔记采用 [知识共享署名—非商业性使用—相同方式共享 4.0 国际许可协议](https://creativecommons.org/licenses/by-nc-sa/4.0/) 授权。  

[![CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
