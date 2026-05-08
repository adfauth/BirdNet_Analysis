This repository contains the files used in a experiment testing differences in species detection and durability based on two different AudioMoth (acoustic recorder) enclosures (Ziplock bags and manufactured cases).

The analysis was used for my Biology Honor's SYE thesis.


Files:

 - baggie_case_analysis.qmd: 
    Contains all the figures and statistical tests that were used in the thesis. 

 - analyze_single_folder.py:
  - script to run BirdNET-Analyzer using the python library birdnetlib
 
 - test_birdnet.run:
  - script to run BirdNET on ada (HPC)

 - code_appendix:
    Contains code from Merging_output.qmd and analyze_single_folder.py

 - figures.qmd (if not deleted) is junk

 - historical_analysis.qmd:
  - failed analysis looking at if the deployment history influence the recording length of recorders during the experiment

 - data_exploration.qmd & prelim_analysis.qmd:
  - mostly junk now, but my initial exploration of the data




Future Directions:

 - need to do valiation on BirdNET data
  - follow sub-sampling method outlined in Thomson et al. 2024
  - REMEMBER: the BirdNET was thresholded at 0.4
  - might need to re-run the BirdNET analysis without any threshold so valiation is more accurate 
 
 - look back at species list sent to local experts to refine data analysis
  - talk to Sue as well about which birds should be left out from original analysis
  - might want to re-run BirdNET without a species list to see how many species it misidentifies 

 - remove the Ziplock at the Cranberry Lake paired site that failed early

 - talk to Cornell Lab of Ornothology to ask some questions about BirdNET
  - can we train BirdNET on our data?
  - is there a better way to contrain the birds BirdNET is choosing from?
   - REMEMBER: the species list just removes birds from the analysis (at least that is what we think)
  - does BirdNET struggle with identifying two species at the same time?
  - what are the best practices in terms of the size of the soundbytes where BirdNET makes its prediction?





