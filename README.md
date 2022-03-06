# freestyleRapSoftware
*Note: To run the chaos theory version of this software, please run the "chaosTheory.ipynb" jupyter notebook; alternatively, for the collapsed gibbs sampler simulation-based method, run "main-Copy1.ipynb". Thank you.
- I obtained my rap lyrics dataset from MCFlow (Condit-Schultz, 2016) and used a text processing function from humdrumR that I created to translate a character vector of syllables to word format.
- This version of Freestyle Rap Software was made in Jupyter Notebook, Python version 3.8.3, and R version 4.1.2. I was initially using JupyterLab then started fiddling around with ipywidgets so that I could get interactive 3D graphs, and this was only possible with earlier versions of Matplotlib and ipywidgets. I tried upgrading again, but the widgets were no longer displaying in JupyterLab, so Jupyter Notebook will have to do for now. I actually like the layout of Jupyter Notebook better anyway, so maybe it works out for the best!
- Refer to pgs 1-2 of the user guide of ipywidgets if you are using Jupyter Notebook (or JupyterLab) and having trouble using ipywidgets: https://ipywidgets.readthedocs.io/_/downloads/en/7.6.3/pdf/

Program instructions and details:
- The user can determine initial values of the volume, rate of speech, and voice type for each set of n rap lines. Then, a collapsed gibbs sampler will 
sample n-1 (since the first values are already determined) 3D multivariate normal samples of values for each variable and assign them to each line i.
- Some rap lines may be read "silently" due to the nature of improvisation, the randomness inherent in this software, and the importance of silence in music.
- To view the mathematics behind the collapsed gibbs sampler method, please refer to my repository labeled "CollapsedGibbsSampler".
