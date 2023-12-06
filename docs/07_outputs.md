Outputs files may be aggregated including information for all samples or provided per sample. Per-sample files will be prefixed with respective aliases and represented below as {{ alias }}.

| Title | File path | Description | Per sample or aggregated |
|-------|-----------|-------------|--------------------------|
| workflow report | ./wf-mpx-report.html | The report for the workflow | aggregated |
| Assembly FASTQ | ./{{ alias }}.final.fastq | Sequence and quality score for final assembly. | per-sample |
| Consensus assembly FASTA | ./consensus.fasta | De-novo consensus assembly sequence from flye and polished by medaka. | per-sample |
| Draft consensus FASTA | ./{{ alias }}.draft.consensus.fasta | Draft consensus sequence from bcftools. | per-sample |
| Read Stats | ./{{ alias }}.per-read-stats.tsv.gz | A simple text file providing a summary of sequencing reads. | per-sample |
| Read alignment | ./{{ alias }}.bam | Read alignments in BAM format. | per-sample |
| Variants file | ./{{ alias }}.annotate.filtered.vcf | Called variants in VCF format. | per-sample |