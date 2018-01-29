# Vulnerability of Biometric Systems to Attacks based on Morphed Biometric Information

Implementation of the framework to predict the vulnerability of biometric systems to attacks using morphed biometric information [[BMT18]](https://doi.org/10.1049/iet-bmt.2017.0144):

## License
This work is licensed under license agreement provided by Hochschule Darmstadt ([h_da-License](/hda-license.pdf)).


## Instructions

### Dependencies
* seaborn
* numpy
* pylab
* matplotlib
* argparse
* csv

### Usage

1. Run evaluateMorphingVulnerability.py

	```python
	usage: evaluateMorphingVulnerability.py [-h] [--fmr [FMR]]
                                        	[--figureTitle [FIGURETITLE]]
                                        	[--legendLocation [LEGENDLOCATION]]
                                        	matedScoresFile nonMatedScoresFile
                                        	figureFile
	
	Evaluate the vulnerability of biometric systems to attacks using morphed
	biometric information.

	positional arguments:
	  matedScoresFile       filename for the mated scores
	  nonMatedScoresFile    filename for the non-mated scores
	  figureFile            filename for the output figure
	
	optional arguments:
	  -h, --help            show this help message and exit
	  --fmr [FMR]           FMR in percentage of the verification threshold, if
	                        none provided, FMR = 0.1 per cent
	  --figureTitle [FIGURETITLE]
	                        title for the output figure
	  --legendLocation [LEGENDLOCATION]
	                        legend location
	```

2. Input: at least 2 score files (mated and non-mated score examples provided), and the file name for the output figure, and optionally other parameters of the computation and the formatting of the figure.

	The score files contain the subject IDs being compared followed by the resulting comparison score, separated by blank spaces. They should be stored as a csv or text file, which will be processed with the [csv package](https://docs.python.org/3/library/csv.html). Examples are provided.

3. Output: figure with score distributions and resulting Pmorph.


## References

More details in:

- [[BMT18]](https://doi.org/10.1049/iet-bmt.2017.0144) M. Gomez-Barrero, C. Rathgeb, U. Scherhag, C. Busch, "Predicting the Vulnerability of Biometric Systems to Attacks based on Morphed Biometric Information", in IET Biometrics, 2018.

Please remember to reference article [[BMT18]](https://doi.org/10.1049/iet-bmt.2017.0144) on any work made public, whatever the form,
based directly or indirectly on these metrics.
