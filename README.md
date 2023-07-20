<p align="center">
<br>
<img src="media/psi4numpybanner.png" alt="Psi4NumPy banner logo" height=200> <br>
<a href="https://zenodo.org/badge/latestdoi/22622192"> <img src="https://zenodo.org/badge/22622192.svg" /></a>
<a href="https://travis-ci.org/psi4/psi4numpy"><img src="https://travis-ci.org/psi4/psi4numpy.svg?branch=master"></a>
<a href="https://codecov.io/gh/psi4/psi4numpy"> <img src="https://codecov.io/gh/psi4/psi4numpy/branch/master/graph/badge.svg" /></a>
<a href="https://opensource.org/licenses/BSD-3-Clause"><img src="https://img.shields.io/badge/License-BSD%203--Clause-blue.svg" /></a>
<br>
<a href="#"> <img src="https://img.shields.io/github/release/psi4/psi4numpy.svg" /></a>
<a href="#"> <img src="https://img.shields.io/github/commits-since/psi4/psi4numpy/latest.svg" /></a>
<a href="#"> <img src="https://img.shields.io/github/release-date/psi4/psi4numpy.svg" /></a>
<a href="#"> <img src="https://img.shields.io/github/commit-activity/y/psi4/psi4numpy.svg" /></a>
<br>
</p>

---

### Overview

开始接触正规的DFT软件，重点关注代码实现，不必深究物理细节

学完这个记得去看GPAW（gitlab仓库已fork，内核不会变，无需更新），充分理解后，可以考虑看非python写的软件包的源码

> What I cannot create, I do not understand. - Richard Feynman

The overall goal of the Psi4NumPy project is to provide an interactive quantum chemistry
framework for reference implementations, rapid prototyping, development, and education.
To do this, quantities relevant to quantum chemistry are computed with the
<span style="font-variant:small-caps;"> Psi4 </span> electronic structure package, and subsequently manipulated 
using the Numerical Python (NumPy) package.  This combination
provides an interface that is both simple to use and remains relatively fast
to execute. 

A series of short scripts demonstrating the implementation of Hartree-Fock Self-Consistent 
Field, SCF Response, Møller-Plesset Perturbation Theory, Symmetry-Adapted Perturbation Theory, 
Coupled Cluster Theory, and more are provided for the reference of the quantum chemistry
community at large to facilitate both reproducibility and low-level methodological understanding.
Additionally, the Tutorials folder above represents an interactive educational
environment containing modules discussing the theory and implementation of various
quantum and computational chemistry methods.  By leveraging the popular Jupyter Notebook
application, each tutorial is constructed as hybrid theory and programming in an easy to use
interactive environment, removing the gap between theory and implementation.

If you have comments, questions, or would like to contribute to the project
please see our [contributor guidelines](https://github.com/psi4/psi4numpy/blob/master/CONTRIBUTING.md).

### Getting Started

在linux上，直接conda安装即可（不需要登录anaconda）

```sh
conda create -n p4env psi4 -c psi4
```
windows上，先禁用镜像，然后

```sh
conda create -n p4env psi4 python=3.8 -c conda-forge/label/libint_dev -c conda-forge
```

### Repository Organization

This repository contains

* reference implementations, which provide working Python scripts implementing
various quantum chemical methods, and
* interactive tutorials, which provide Jupyter notebooks presenting a hybrid
theory-and-implementation educational framework for learning to program quantum
chemistry methods.

Reference implementations are organized into top-level directories
corresponding to the over-arching theory upon which each method is based, i.e.,
both EOM-CCSD and TD-CCSD are contained in the
[Coupled-Cluster](https://github.com/psi4/psi4numpy/tree/master/Coupled-Cluster)
directory.  All interactive tutorials are contained in the top-level directory
[Tutorials](https://github.com/psi4/psi4numpy/tree/master/Tutorials).  These
tutorials are organized in logical order of progression, which is enumerated in
detail
[here](https://github.com/psi4/psi4numpy/tree/master/Tutorials#interactive-tutorials).

### Psi4 v1.1 (c. May 2017)
This repostitory has recently been updated to be compatible with Psi4 version 1.1.
Please see the [v0.1-beta tag](https://github.com/psi4/psi4numpy/tree/v0.1-beta) for a Psi4 v1.0 compliant Psi4NumPy version. 

### Psi4 v1.2 (c. May 2018)
This reposititory is fully compatible with the upcoming Psi4 version 1.2.
In fact (for a while), if you use v1.2, there's no need to worry if your Psi4 has
all the features to run all the reference implementations and tutorials.

### Citation
Please consider citing this repository through the Psi4NumPy paper:

Psi4NumPy: An Interactive Quantum Chemistry Programming Environment for Reference Implementations and Rapid Development
Daniel G. A. Smith, Lori A. Burns, Dominic A. Sirianni, Daniel R. Nascimento, Ashutosh Kumar, Andrew M. James, Jeffrey B. Schriber, Tianyuan Zhang, Boyi Zhang, Adam S. Abbott, Eric J. Berquist, Marvin H. Lechner, Leonardo A. Cunha, Alexander G. Heide, Jonathan M. Waldrop, Tyler Y. Takeshita, Asem Alenaizan, Daniel Neuhauser, Rollin A. King, Andrew C. Simmonett, Justin M. Turney, Henry F. Schaefer, Francesco A. Evangelista, A. Eugene DePrince III, T. Daniel Crawford, Konrad Patkowski, and C. David Sherrill
*Journal of Chemical Theory and Computation*, **2018**, 14 (7), 3504-3511
DOI: 10.1021/acs.jctc.8b00286
