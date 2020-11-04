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

- A validation report in text format containing the stdout

