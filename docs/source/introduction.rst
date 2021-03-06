Introduction
============

**QuantumOptics.jl** is a numerical framework written in `Julia <http://julialang.org/>`_ that makes it easy to simulate various kinds of quantum systems. It is similar to the `Quantum Optics Toolbox <http://qo.phy.auckland.ac.nz/toolbox/>`_ for MATLAB and its Python equivalent `QuTiP <http://qutip.org/>`_.

One of the core concepts of **QuantumOptics.jl** is that all quantum objects, i.e. state vectors and operators have knowledge about which Hilbert space they live in. This prevents many common mistakes when working with composite systems and at the same time improves readability. The Hilbert spaces are defined implicitly by specifying appropriate bases like :ref:`fock <section-fock>` bases and :ref:`spin <section-spin>` bases. These bases can in turn be combined to describe composite systems like e.g. a particle in a cavity or a multi-spin system. Working with bases is explained in great detail in the :ref:`section-bases` section.

After choosing a basis **QuantumOptics.jl** provides many useful functions to create common :ref:`section-operators` and :ref:`section-states` which can be combined in all the expected ways. Consequently, constructing arbitrary Hamiltonians and Liouvillians and specifying initial states is straight forward. These objects can be used to perform time evolutions according to :ref:`Schroedinger <section-schroedinger>`, :ref:`Master <section-master>` and :ref:`Monte Carlo wave function <section-mcwf>` equations.

Although the main focus is on simulating dynamics of (open) quantum systems, there are nevertheless many additional features available to calculate :ref:`steadystates <section-steadystate>`, the :ref:`energy spectrum, eigenstates <section-spectralanalysis>`, and :ref:`correlation functions <section-correlationfunctions>`.
