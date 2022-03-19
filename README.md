# vvcsem
TIME DOMAIN MODELING – VVCSEM EXAMPLE

When it comes to electrical and electromagnetic computational modeling, the difficulties are the mathematical formulations that describe the events that one wants to represent/analyze, as well as the field behavior, its components in different media and, mainly, transient behavior in the field measurements. Thus, a number of professionals and even companies dedicated and dedicated their research to the development and improvement of codes in different languages and platforms.

The main objective and contribution of our manuscript is to show how the analysis of the behavior of electromagnetic fields can be done without great knowledge of scientific programming or monetary costs with applications with proprietary softwares.

The code was written within Jupyter notebooks in Anaconda, which is a free distribution platform for the Python programming language. In Anaconda, codes are built (or imported from modules) and compiled in the same environment in which the figures are plotted (matplotlib), in addition to providing a user-friendly interface, besides the reduction in time and computational capacity. A time domain method was used because for many it is still a barrier, since we have more affinity with frequency domain methods.

For models with vertical transverse isotropy (VTI), we highlight the modeling code, EMmod (Hunziker et al., 2015) which was built using Fortran language. And EMPYMOD (Werthmüller, 2017) and EMG3D (Werthmüller et al., 2021), which was based on EMmod, formulated in Python language and which is hosted in the GitHUB repository. Helping to obtain results in the domain of frequency and time, purpose of this publication.

The present data set shows the code that was used to generate of the time domain modeling of the VVCSEM method. The code used was built in the Jupyter notebook from routines contained in the example of the modeling of the MCSEM method made in EMPYMOD and made available on GitHub. EMPYMOD (Werthmüller et al., 2021) is an open-source full 3D electromagnetic modeller for 1D VTI media. It was developed in Python and the program developed for VVCSEM takes advantage of the electromagnetic field solution in a canonical model, changing the source (Tx) from dipole to bipole, frequency domain to time domain (FFT and Hankel), source and receiver orientation from horizontal to vertical, in addition to the EM field component from Ex to Ez.

1. **Conda**:

        conda install -c prisae empymod
    
   If you are using the Anaconda Navigator, just add the channel `prisae` and empymod will appear in the package list.

2. **Pip**:

        pip install empymod
    
3. Download, clone, or fork on **GitHub**: [github.com/prisae/empymod](https://github.com/prisae/empymod).
   To install it run

        python setup.py install

   or simply put it in your working directory or Python-PATH to use it without installation at all.
