# MB-GAN

Microbiome Simulation via Generative Adversarial Network


### Introduction

MB-GAN is a deep learning simulation framework for simulating realistic
microbiome data

Manuscript is avaialble at bioRxiv https://doi.org/10.1101/863977

### Information provided by this repository

##### Data folder

The folder “data” contains:

  - The real microbiome data used to generate MB-GAN samples analyzed in
    the manuscript

  - The csv files of the MB-GAN samples

  - The simulated data by alternative methods: Normal-To-Anything and metaSPARSim
  
  - The processed data used to generate figures and tables in the
    manuscript

##### R codes

The folder “Rcode” includes the following R scripts:

  - `generate_NorTA.R`: Simulate data by Normal-To-Anything (NorTA)
  
  - `generate_metaSPARSim.R`: Simulate data by metaSPARSim
  
  - `process_MBGAN.R`: Converts the csv files of MB-GAN samples to
    `Rdata` files
    
  - `calculate_unifrac_dist.R`: Calculate UniFrac distance for real microbiome samples and samples generated by three simulation methods (MBGAN, NorTA, metaSPARSim)
  
  - `check_first_level_property.R`: Compare sample sparsity, abundance, alpha diversity (by Shannon index), and beta diversity (by non-metric multidimensional scaling (nMDS) analysis)
  
  - `check_second_level_property.R`: Compare taxa-taxa associations using correlation structure and proportionality 
  
  - `check_second_level_property.R`: Compare differential abundance analysis results based on the real microbiome and MBGAN simulated samples
  
  - `MiRKAT_simulation.R` and `MiRKAT_result_summary.R`: Implement MiRKAT using MBGAN samples
  
  - `generate_abundance_heatmap.R`: Compare the abundances of the top 60 most abundant taxa across different datasets


The folder “Rcode_smalldataset” includes the similar R codes as above for the small microbiome dataset dicussed in the supplement.

##### Python codes

The root folder includes the following Python scripts:

  - `mbgan_train_demo.py`: codes to train a MB-GAN network
  - `mbgan_inference_casectrl.py`: codes to simulate new microbiome 
    abundances using trained model parameters
    
The folder "code_check_convergence" includes Python scripts to validate the model convergence.

The folder "models" includes the trained model weights.

The folder "outputs" includes simulation outputs.
    
The folder "models_smaller_dataset" includes the following Python scripts (similar to above):

  - `inference_case_ctrl.py`: codes to simulate new microbiome 
    abundances for the smaller microbiome dataset using trained model parameters



## Contact

Xiaowei Zhan <xiaowei.zhan@utsouthwestern.edu>
Quantitative Biomedical Research Center
Center for the Genetics of Host Defence
Department of Population and Data Sciences
UT Southwestern Medical Center
Dallas, TX 75390-8821
