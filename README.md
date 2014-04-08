GromacsIPython
==============

Using Gomacs from IPython notebook.
This is not a complete tutorial on how to use GROMACS (refer f.e. to excelent [tutorials](http://www.bevanlab.biochem.vt.edu/Pages/Personal/justin/gmx-tutorials/)).
The goal of this repository is to provide an indea that using
IPython is beneficial to your work. You can instantly visualize results, all your protocols are saved in one place, and the overall 
structure of the notebook makes using gromacs more straightforward.

The peptide we want to model is a small part of [Apoliprotein A1](http://en.wikipedia.org/wiki/Apolipoprotein_A1) (1ODQ). The first step after I downloaded
it from PDB databank (http://rcsb.org) was to save a single model from multimodel file. Therefore the file 1ODQ.pdb contains only one of many models
of this peptide.

**Preprequisites:**

1. GROMACS
2. IPython
3. Prettyplotlib (depends on matplotlib 1.2-1.3)
4. Pymol
5. mencoder and ffmpeg to make and convert MD video

**The steps are the following:**
1. [Generating the topology of the structure, solvating, adding ions and minimizing](http://nbviewer.ipython.org/github/lupoglaz/GromacsIPython/blob/master/EnergyMinimization.ipynb?create=1)
2. [NVT and NPT coupling](http://nbviewer.ipython.org/github/lupoglaz/GromacsIPython/blob/master/TemperatureAndPressureCoupling.ipynb?create=1)
3. [MD production](http://nbviewer.ipython.org/github/lupoglaz/GromacsIPython/blob/master/RunMD.ipynb?create=1)
4. [Analysis and visualization of MD](http://nbviewer.ipython.org/github/lupoglaz/GromacsIPython/blob/master/MDAnalysis.ipynb?create=1)


All the notebooks include one script file called IPythonTweaks.py. It contains different drawing procedures used throughout the notebooks.

Note: The code of scripts is currently quite raw, and be carefull applying it tou your projects. I hope I will be gradually updating it
with time.
