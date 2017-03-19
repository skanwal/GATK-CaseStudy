# Instructions to run CWL workflow:
1. Install the specific version of cwltool used in this analysis using pip:
    *  *pip install cwltool==1.0.20150915034626*
    
2. Download the CWL specifications for tools and workflow along with the JSON file used in the analysis from https://swift.rc.nectar.org.au:8888/v1/AUTH_377/Paper-Data/WorkflowFiles/GATK-CWL-WorkflowFiles.tar.gz.

3. Download input data provided and modify the JSON file (*GATK-complete-Workflow.json*) to add paths for the input, reference sequence (*hg19.fasta*) and known variant files. Make sure to download the index files (_hg19.fasta.*_) provided along with the reference sequence and place them in the same directory as *hg19.fasta*.

4. In addition create a temporary directory (TEMPDIR) in the current working directory which will be used further in the command (as shown in sample command).

5. Run the analysis using the following sample command:
    * *cwltool --debug --tmpdir-prefix=PATH_TO/CURRENTDIR/TEMPDIR --tmp-outdir-prefix PATH_TO/CURRENTDIR/TEMPDIR ./GATK-complete-Workflow.cwl ./GATK-complete-Workflow.json*
