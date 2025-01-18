---
layout: page
title: projects
permalink: /projects/
# description:
nav: true
nav_order: 4
---


# Projects

This page highlights my research-driven projects. I frequently update it with
relevant materials as my work progresses.

- [Project: FauxPy](#project-fauxpy)
- [Project: aNNoTest](#project-annotest)

## Project: FauxPy

FauxPy is the first multi-family fault localization tool for Python programs,
available as open-source software. The current version of FauxPy supports the
following fault localization families:
- Spectrum-Based Fault Localization
- Mutation-Based Fault Localization
- Predicate Switching
- Stack Trace Fault Localization

Fault localization refers to automated techniques that help developers identify
buggy locations within their codebase. These techniques typically produce a
ranked list of program entities (e.g., statements, functions/methods, files).
Developers or [automated program repair](https://program-repair.org) tools can
use this list, starting with the highest-ranked entity (most likely to contain
the bug), and continue until the bug is located and resolved.

FauxPy is a dynamic analysis tool that has been tested on 135 real-world bugs
across 13 well-known projects, demonstrating its robustness and effectiveness.
Below is a complete list of projects FauxPy has been tested with:

- [black](https://github.com/psf/black)
- [cookiecutter](https://github.com/cookiecutter/cookiecutter)
- [fastapi](https://github.com/tiangolo/fastapi)
- [httpie](https://github.com/jakubroztocil/httpie)
- [keras](https://github.com/keras-team/keras)
- [luigi](https://github.com/spotify/luigi)
- [pandas](https://github.com/pandas-dev/pandas)
- [sanic](https://github.com/huge-success/sanic)
- [spaCy](https://github.com/explosion/spaCy)
- [thefuck](https://github.com/nvbn/thefuck)
- [tornado](https://github.com/tornadoweb/tornado)
- [tqdm](https://github.com/tqdm/tqdm)
- [youtube-dl](https://github.com/ytdl-org/youtube-dl)

### Key Links

- [Source Code](https://github.com/atom-sw/fauxpy)
- [Documentation](https://fauxpy.readthedocs.io)
- [Experiments on Real-World Bugs](https://github.com/atom-sw/fauxpy-experiments)
- [Demo Video of FauxPy in Action](https://www.youtube.com/watch?v=6ooPPiwd79g)

### Publications

1. **An empirical study of fault localization in Python programs**
   *Mohammad Rezaalipour and Carlo A. Furia*
   Published in *Empirical Software Engineering*, Volume 29, Issue 4, 2024, Pages 92
   - DOI: [10.1007/s10664-024-10475-3](https://doi.org/10.1007/s10664-024-10475-3)

2. **FauxPy: A Fault Localization Tool for Python**
   *Mohammad Rezaalipour and Carlo A. Furia*
   arXiv Technical Report, 2024
   - arXiv: [2404.18596](https://arxiv.org/abs/2404.18596)

## Project: aNNoTest

aNNoTest is an annotation-based test generation approach and tool specifically designed
for Python-based neural network programs. Using annotations written in aN—a
concise and descriptive annotation language that we developed—aNNoTest generates
[Hypothesis](https://hypothesis.readthedocs.io) test templates for functions,
methods, and modules within a neural network program, which can then be run to
identify bugs.

aNNoTest has been evaluated on 19 real-world programs and has successfully
identified several previously unknown bugs and reproduced many known bugs,
highlighting its bug-finding capabilities. Notably, aNNoTest discovered [one
bug](https://github.com/pytorch/vision/issues/5209) and [one documentation
inconsistency](https://github.com/pytorch/vision/issues/6607) in
[Vision](https://github.com/pytorch/vision), PyTorch's machine vision library.
Both issues were accepted by the maintainers and integrated into the library’s
codebase.

### Key Links

- [Source Code](https://github.com/atom-sw/annotest)
- [Dataset of Real-World Neural Network Bugs](https://github.com/atom-sw/annotest-subjects)

### Publications

1. **aNNoTest: An Annotation-based Test Generation Tool for Neural Network Programs**
   *Mohammad Rezaalipour and Carlo A. Furia*
   Proceedings of the 39th IEEE International Conference on Software Maintenance
   and Evolution (ICSME), 2023, Pages 574–579
   - DOI: [10.1109/ICSME58846.2023.00075](https://doi.org/10.1109/ICSME58846.2023.00075)

2. **An annotation-based approach for finding bugs in neural network programs**
   *Mohammad Rezaalipour and Carlo A. Furia*
   Published in *Journal of Systems and Software*, Volume 201, 2023, Pages 111669
   - DOI: [10.1016/j.jss.2023.111669](https://doi.org/10.1016/j.jss.2023.111669)
