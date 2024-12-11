---
layout: page
title: publications
permalink: /publications/
description: My publications by categories in reversed chronological order.
nav: true
nav_order: 2
---

##### Journal Articles

- [An empirical study of fault localization in Python programs](#an-empirical-study-of-fault-localization-in-python-programs)
- [Doctor Code: A machine learning-based approach to program repair](#doctor-code-a-machine-learning-based-approach-to-program-repair)
- [An annotation-based approach for finding bugs in neural network programs](#an-annotation-based-approach-for-finding-bugs-in-neural-network-programs)
- [AxMAP: Making Approximate Adders Aware of Input Patterns](#axmap-making-approximate-adders-aware-of-input-patterns)
- [IDrAx: A tool-chain for designing efficient approximate adders](#idrax-a-tool-chain-for-designing-efficient-approximate-adders)

##### Conference Proceedings

- [aNNoTest: An Annotation-based Test Generation Tool for Neural Network Programs](#annotest-an-annotation-based-test-generation-tool-for-neural-network-programs)
- [An Approach to Generate Effective Fault Localization Methods for Programs](#an-approach-to-generate-effective-fault-localization-methods-for-programs)
- [Arselda: An Improvement on Adaptive Random Testing by Adaptive Region Selection](#arselda-an-improvement-on-adaptive-random-testing-by-adaptive-region-selection)

##### Technical Reports

- [FauxPy: A Fault Localization Tool for Python](#fauxpy-a-fault-localization-tool-for-python)

##### PhD Thesis

- [Test case generation and fault localization for data science programs](#test-case-generation-and-fault-localization-for-data-science-programs)

---

## Details

---

#### An empirical study of fault localization in Python programs

Mohammad Rezaalipour and Carlo A. Furia  
Empirical Software Engineering  
2024  

**Abstract:**

Despite its massive popularity as a programming language, especially in novel domains like data science programs, there is comparatively little research about fault localization that targets Python. Even though it is plausible that several findings about programming languages like C/C++ and Java—the most common choices for fault localization research—carry over to other languages, whether the dynamic nature of Python and how the language is used in practice affect the capabilities of classic fault localization approaches remain open questions to investigate.

This paper is the first multi-family large-scale empirical study of fault localization on real-world Python programs and faults. Using Zou et al.’s recent large-scale empirical study of fault localization in Java (Zou et al. 2021) as the basis of our study, we investigated the effectiveness (i.e., localization accuracy), efficiency (i.e., runtime performance), and other features (e.g., different entity granularities) of seven well-known fault-localization techniques in four families (spectrum-based, mutation-based, predicate switching, and stack-trace based) on 135 faults from 13 open-source Python projects from the BugsInPy curated collection (Widyasari et al. 2020).

The results replicate for Python several results known about Java, and shed light on whether Python’s peculiarities affect the capabilities of fault localization. The replication package that accompanies this paper includes detailed data about our experiments, as well as the tool FauxPy that we implemented to conduct the study.


- DOI: [10.1007/s10664-024-10475-3](https://doi.org/10.1007/s10664-024-10475-3)
- arXiv: [2305.19834](https://arxiv.org/abs/2305.19834)
- GitHub page: [https://github.com/atom-sw/fauxpy-experiments](https://github.com/atom-sw/fauxpy-experiments)
- FauxPy tool: [https://fauxpy.readthedocs.io](https://fauxpy.readthedocs.io)

---

#### Doctor Code: A machine learning-based approach to program repair

Sharmin Moosavi, Mojtaba Vahidi-Asl, Hassan Haghighi, and Mohammad Rezaalipour  
Scientia Iranica  
2024

**Abstract:**

To address the problems of automatic repair techniques, we present Doctor Code, a new APR technique that chooses repair operators by systematically learning from the features of the most common bugs in different programs, using machine learning. The wise selection of repair operators reduces the number of candidate patches. We compare our technique against Mutation repair, a test suite-based APR technique, using the Siemens suite. The experiment results indicate that our technique can fix 41 bugs while the baseline only repairs 22. In addition, Doctor Code can produce patches that do not exist in the search space of the three test suite-based techniques called SPR, Prophet, and SemFix. We also experiment with Doctor Code utilizing three buggy versions of a program called Space (9K LOC), to indicate its capability of repairing large-sized programs. In addition, we compare Doctor Code against 7 state-of-the-art APR tools like Elixir, using the Defects4j dataset. The experiment results indicate that our technique outperforms the other tools regarding the number of fixed bugs and overfitted patches.

Comparing Doctor Code with RAPR as the baseline indicates that using machine learning reduces the number of overfitted patches and the time of patch production by 33.33% and 82.68%, respectively.

- DOI: [10.24200/sci.2023.54718.3884](https://doi.org/10.24200/sci.2023.54718.3884)

---

#### Test case generation and fault localization for data science programs

Mohammad Rezaalipour  
PhD Thesis, Università della Svizzera italiana  
2024

**Abstract:**

Data science refers to inter-disciplinary approaches designed to extract knowledge from vast amounts of data. It combines techniques from fields such as statistics and machine learning to develop novel applications for different science and engineering domains. Data science approaches are implemented as programs usually written in languages such as R or Python, collectively referred to as data science programs. Due to their inter-disciplinary usages, these programs are often written by domain experts possibly unfamiliar with the best practices of software development, and thus, they may exhibit low quality. In fact, there is evidence that these programs contain several bugs, often different in nature compared to those found in traditional programs. As a result, data science programs challenge conventional debugging techniques such as those from test generation and fault localization activities, due to the unique nature of bugs found in them. Additionally, being written in dynamically typed languages such as Python adds to the difficulties of testing and analyzing them.

These challenges call for research into new debugging techniques tailored specifically for these programs, which is the focus of the current dissertation. Precisely, this thesis aims to understand the capabilities and limitations of standard test generation and fault localization techniques on data science programs implemented in dynamic languages such as Python. To achieve this goal, the dissertation presents contributions in three areas: i) a test generation technique for neural network (NN) programs, a wide spread class of data science programs; ii) an empirical study of fault localization in Python programs; and iii) two debugging tools and a curated dataset of NN bugs.

In the first area, we investigated and identified the limitations of general-purpose test generation techniques on NN programs, which led to the development of aNNoTest, a novel test generation technique tailored for NN programs. We evaluated aNNoTest on 19 open-source programs, demonstrating its effectiveness at finding bugs in real-world NN programs. In the second area, we conducted the first large-scale multi-family empirical study of fault localization in Python programs. Targeting 135 bugs from 13 projects, we studied seven fault localization techniques from four families along with combinations of them. We considered different fault localization granularity levels and measured both effectiveness and efficiency in our analyses. In the third area, we developed: i) the aNNoTest tool, an implementation of the aNNoTest approach mentioned above; ii) FauxPy, to our knowledge, the first open-source multi-family fault localization tool for Python; and iii) a curated dataset of NN bugs, for which aNNoTest was used to generate tests.

Along with supporting the domain with the tools and techniques we developed, we hope our contributions will be beneficial to inform the development of more effective debugging techniques for Python data science programs.

- URN: [urn:nbn:ch:rero-006-122207](https://n2t.net/ark:/12658/srd1328869)

---

#### FauxPy: A Fault Localization Tool for Python

Mohammad Rezaalipour and Carlo A. Furia  
arXiv Technical Report  
2024

**Abstract:**

This paper presents FauxPy, a fault localization tool for Python programs. FauxPy supports seven well-known fault localization techniques in four families: spectrum-based, mutation-based, predicate switching, and stack trace fault localization. It is implemented as plugin of the popular Pytest testing framework, but also works with tests written for Unittest and Hypothesis (two other popular testing frameworks). The paper showcases how to use FauxPy on two illustrative examples, and then discusses its main features and capabilities from a user's perspective. To demonstrate that FauxPy is applicable to analyze Python projects of realistic size, the paper also summarizes the results of an extensive experimental evaluation that applied FauxPy to 135 real-world bugs from the BugsInPy curated collection. To our knowledge, FauxPy is the first open-source fault localization tool for Python that supports multiple fault localization families.

- arXiv: [2404.18596](https://arxiv.org/abs/2404.18596)
- FauxPy documentation: [https://fauxpy.readthedocs.io](https://fauxpy.readthedocs.io)

---

#### aNNoTest: An Annotation-based Test Generation Tool for Neural Network Programs

Mohammad Rezaalipour and Carlo A. Furia  
Proceedings of the 39th IEEE International Conference on Software Maintenance and Evolution (ICSME)  
2023

**Abstract:**

Even though neural network (NN) programs are often written in Python, using general-purpose test-generation tools for Python to test them is likely to be ineffective, as these tools do not support the particular input constraints that NN programs often require. To address this challenge, we present aNNoTest: an automated unit-test generation tool for NN programs written in Python. aNNoTest offers a simple annotation language that is suitable to concisely express the usual input constraints of NN programs; it then uses these annotations to precisely generate valid inputs that are capable of revealing bugs. This short paper describes how aNNoTest works in practice, and reports some experiments that demonstrate its effectiveness as a bug-finding tool for NN programs. aNNoTest is available as open source.

- DOI: [10.1109/ICSME58846.2023.00075](https://doi.org/10.1109/ICSME58846.2023.00075)
- aNNoTest tool: [https://github.com/atom-sw/annotest](https://github.com/atom-sw/annotest)
- Curated dataset or NN bugs: [https://github.com/atom-sw/annotest-subjects](https://github.com/atom-sw/annotest-subjects)

---

#### An annotation-based approach for finding bugs in neural network programs

Mohammad Rezaalipour and Carlo A. Furia  
Journal of Systems and Software  
2023

**Abstract:**

As neural networks are increasingly included as core components of safety–critical systems, developing effective testing techniques specialized for them becomes crucial. The bulk of the research has focused on testing neural-network models; but these models are defined by writing programs, and there is growing evidence that these neural-network programs often have bugs too.

This paper presents aNNoTest: an approach to generating test inputs for neural-network programs. A fundamental challenge is that the dynamically-typed languages (e.g., Python) commonly used to program neural networks cannot express detailed constraints about valid function inputs (e.g., matrices with certain dimensions). Without knowing these constraints, automated test-case generation is prone to producing invalid inputs, which trigger spurious failures and are useless for identifying real bugs. To address this problem, we introduce a simple annotation language tailored for concisely expressing valid function inputs in neural-network programs. aNNoTest takes as input an annotated program, and uses property-based testing to generate random inputs that satisfy the validity constraints. In the paper, we also outline guidelines that simplify writing aNNoTest annotations.

We evaluated aNNoTest on 19 neural-network programs from Islam et al’s survey. Islam et al. (2019), which we manually annotated following our guidelines — producing 6 annotations per tested function on average. aNNoTest automatically generated test inputs that revealed 94 bugs, including 63 bugs that the survey reported for these projects. These results suggest that aNNoTest can be a valuable approach to finding widespread bugs in real-world neural-network programs.

- DOI: [10.1016/j.jss.2023.111669](https://doi.org/10.1016/j.jss.2023.111669)
- aNNoTest tool: [https://github.com/atom-sw/annotest](https://github.com/atom-sw/annotest)
- Curated dataset or NN bugs: [https://github.com/atom-sw/annotest-subjects](https://github.com/atom-sw/annotest-subjects)

---

#### AxMAP: Making Approximate Adders Aware of Input Patterns

Morteza Rezaalipour, Mohammad Rezaalipour, Masoud Dehyadegari, and Mahdi Nazm Bojnordi  
IEEE Transactions on Computers  
2020

**Abstract:**

Making approximate computing specific to user requirements is crucial to system performance, energy-efficiency, and reliability. However, developing hardware for such optimization becomes a significant challenge due to the high cost of examining all potential choices while exploring a large design space. One determinant aspect of exploring a design space is the efficiency of evaluating error metrics, such as the Mean Error Distance (MED) and the Error Probability (EP), for each possible choice within the search space. Since computing these error-metrics is quite time-consuming, efficient calculation approaches are essential. This article proposes a novel formal approach to accurately compute the EP and MED of approximate adders for any input pattern at a linear time and space complexity. Our experimental results indicate that the proposed approach can accurately compute the error-metrics of large approximate adders at a 150 times faster speed compared to the Monte Carlo sampling methods. We then develop AxMAP, a design tool based on the proposed error-metrics computation that generates energy-efficient approximate adders for any given input pattern. When applied to image processing applications, AxMAP produces more than 150 different designs for adders that achieve superior performance and energy-efficiency compared to the existing state-of-the-art approximate adders.

- DOI: [10.1109/TC.2020.2968905](https://doi.org/10.1109/TC.2020.2968905)
- GitHub page: [https://github.com/mohrez86/AxMAP](https://github.com/mohrez86/AxMAP)

---

#### IDrAx: A tool-chain for designing efficient approximate adders

Morteza Rezaalipour, Mohammad Rezaalipour, Sarvenaz Tajasob, and Masoud Dehyadegari  
Microelectronics Journal  
2019

**Abstract:**

As transistors shrink down, improving the energy-efficiency of nanometer ICs has gained a great deal of attention. Recently, approximate computing has been introduced to address energy-efficiency problems of error-tolerant systems. Adders are the most widely used arithmetic modules that consume significant amounts of system's total energy and area. The error-resiliency of these systems has made it possible to innovate energy-efficiency approximate adders to obtain low power and high-speed circuits. This paper presents IDrAx, an approach to improve the accuracy of approximate adders. The goal is to find the most significant errors in the error distribution for the given circuit and correct them through low-cost additional circuits. The proposed method is applied to several state-of-the-art approximate adders for evaluation by considering two different input distributions. Our simulation results indicate that the proposed design achieves by 75% and 78.01% accuracy regarding mean error distance metric for uniform and normal input distributions, respectively.

- DOI: [10.1016/j.mejo.2019.06.011](https://doi.org/10.1016/j.mejo.2019.06.011)

---

#### An Approach to Generate Effective Fault Localization Methods for Programs

Babak Bagheri, Mohammad Rezaalipour, and Mojtaba Vahidi-Asl  
Fundamentals of Software Engineering  
2019

**Abstract:**

Software Debugging is a tedious and costly task in software development life-cycle. Thus, various automated fault localization approaches have been proposed to address this problem, among which, spectrum-based fault localization has attracted a lot of attention. Using various formulas, known as ranking metrics, spectrum-based fault localization techniques assign scores to the entities of programs (e.g., statements) based on their suspiciousness of being the root cause of failures. Despite the obvious advantages of spectrum-based fault localization techniques, such as being lightweight, they cannot effectively locate faults in every program owing to the fact that they do not consider the characteristics of the programs. We believe that program characteristics can be helpful at finding the right ranking metrics for programs, and they can assist at combining several existing ones to produce a customized ranking metric specific to a given program.

In this paper, we have proposed an approach which combines 40 different ranking metrics to generate a new ranking metric specific to a given program. Employing mutation testing operators, the proposed approach retrieves information from the program and then, using different preferential voting systems, it combines various ranking metrics based on the collected information. We have evaluated our approach on 154 faulty versions from eight different programs of Space and Siemens test suite and compare it with nine state-of-the-art ranking metrics. The experimental results indicate that the ranking metrics generated by our approach is superior with respect to evaluation metrics such as the Exam score and TOP-N.

- DOI: [10.1007/978-3-030-31517-7_17](https://doi.org/10.1007/978-3-030-31517-7_17)

---

#### Arselda: An Improvement on Adaptive Random Testing by Adaptive Region Selection

Mohammad Rezaalipour, Lida Talebsafa, and Mojtaba Vahidi-Asl  
8th International Conference on Computer and Knowledge Engineering (ICCKE)  
2018

**Abstract:**

Distance-aware Forgetting Fixed Size Candidate Set (DF-FSCS) is an Adaptive Random Testing (ART) technique, which lowers the computational overhead of Fixed Size Candidate Set ART (FSCS-ART), using a forgetting strategy. DF-FSCS partitions the input domain into regions, and while computing the distance of a candidate test case from executed test cases, as a vector in the input domain, it only considers test cases that are in the same region as the candidate. Although being a lightweight technique, there are two issues with DF-FSCS. First, it does not attempt to generate test cases in low-density regions, which if done, could result in a more even spread of test cases. Second, the regions it defines are smaller at the lower or upper boundaries of input domains, which declines the quality of test cases produced in these regions.

We propose Arselda, an APR technique that improves DF-FSCS. By generating test cases in low-density regions that have a fewer number of test cases and enlarging regions at lower or upper boundaries of input domains, Arselda addresses the two issues mentioned above. Considering DF-FSCS as the baseline, a simulation analysis has been performed to evaluate the effectiveness of Arselda. According to the experiment results, Arselda has better failure detection effectiveness compared with the baseline for the block failure pattern. Also, Arselda has lower computational overhead than the baseline.

- DOI: [10.1109/ICCKE.2018.8566625](https://doi.org/10.1109/ICCKE.2018.8566625)
