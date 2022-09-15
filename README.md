#How to install the necessary packages for the Mathematica code and open the corresponding notebooks:

1. Add LieAnalysis-package to the right folder:

Download the LieAnalysis-package via [www.LieAnalysis.nl](http://www.lieanalysis.nl/wp-content/uploads/2018/LieAnalysis-25-04-2018.zip)

and put it in the folder "C:\Users\s149687\AppData\Roaming\Mathematica\Applications". Note that your folder path will be slightly different.

2. Install Anaconda3.

3. Install the Fast Marching code. Open "Anaconda Prompt". (Step a is only needed once, after the environment is created, you can start in Step b).

	1. Indented Create Conda environment adg-hfm.

		conda create -n adg-hfm python=3.7 jupyterlab cupy matplotlib scipy

		conda activate adg-hfm

		conda install -c agd-lbr agd hfm

	2. Indented Call adg-hfm from Mathematica. Note that the second line should lead to the folder in which Mathematica is installed. This may be different from the stated suggestion.

		conda activate adg-hfm

		cd\Program Files\Wolfram Research\Mathematica\12.3\

		Mathematica.exe

4. You can now run the notebooks. For the "TrackingVascularTrees_..." notebooks, it is important that the folder "IO_STAR_GT.zip" is unzipped and in the same folder as the notebook that you are working on.