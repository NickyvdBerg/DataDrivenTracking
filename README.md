How to install the necessary packages for the Mathematica code and open the corresponding notebooks:

1. Add LieAnalysis-package to the right folder:
Unzip the folder "LieAnalysis.zip" in the folder "C:\Users\s149687\AppData\Roaming\Mathematica\Applications". Note that your folder path will be slightly different.

2. Install Anaconda3.

3. Install the Fast Marching code. Open "Anaconda Prompt". (Step a is only needed once, after the environment is created, you can start in Step b).
	a) Create Conda environment adg-hfm.
		conda create -n adg-hfm python=3.7 jupyterlab cupy matplotlib scipy
		conda activate adg-hfm
		conda install -c agd-lbr agd hfm

	b) Call adg-hfm from Mathematica. Note that the second line should lead to the folder in which Mathematica is installed. This may be different from the stated suggestion.
		conda activate adg-hfm
		cd\Program Files\Wolfram Research\Mathematica\12.3\
		Mathematica.exe

4. You can now run the notebooks.