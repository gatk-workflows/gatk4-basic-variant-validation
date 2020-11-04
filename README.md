# gatk4-basic-variant-validation
Simple workflow to validate a VCF (or GVCF) -- NOT Best Practices, only for teaching/demo purposes.

## Inputs and outputs 

### Required inputs

- One VCF file or GVCF file and its index (can be bgzip/tabix)
- A list of intervals to process (for parallelization)
- Genomic resources: reference genome in FASTA format (.fasta) and its accessory files (.fasta.fai and .dict)

### Optional inputs 

- Resourcing and environment parameters including memory, disk space and container are all customizable

### Outputs

- A list of text files containing the tool's standard output, which will contain the relevant error message 
  if the tool encounters a validation error. 
  
**Important note:** The tool will produce a non-zero return code if it finds an error. The Cromwell workflow 
management system considers this to mean the workflow failed even if the tool worked properly. In Terra, this 
will cause the workflow to be displayed as having failed, and the standard output file will not be added to 
the data model.

