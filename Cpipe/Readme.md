1. Clone online Cpipe GitHub repository:
      * *git clone https://github.com/MelbourneGenomics/cpipe.git*
      
2. Run the install script:
      * *cd Cpipe*
      * *./pipeline/scripts/install.sh*
      
3. Follow the instructions given in user guide available at to set up directory structure necessary to run the analysis (https://melbournegenomics.github.io/docs/Cpipe_User_Guide.pdf).

4. After setting up the directory structure using Cpipe User Guide, download input data (FQ_1.fastq and FQ_2.fastq) used in this analysis from https://swift.rc.nectar.org.au:8888/v1/AUTH_377/Paper-Data. The sample text file (https://swift.rc.nectar.org.au:8888/v1/AUTH_377/Paper-Data/InputData/samples.txt) used for the analysis is also provided with this data.

5. The pipeline expects a target region bed file (target_region.bed) in the design folder. These are the region that will be reported in the final results. The data used in our analysis was from chromosome 21, hence we didn’t focus on any specific genomic region. Therefore, an empty target_region.bed file was created to successfully run the analysis.

6. The final output of the workflow named as 'Cpipe-broad-filtered.recode.vcf' is provided for comparison of results. 
