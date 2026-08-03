# MB5370 Module 3 Workshop 3

Workshop 3: Metagenome assembly extends the single-genome skills from Workshop 2 to a mock community of five bacterial species, designed to capture key metagenomic challenges like variable species abundance and two closely related, hard-to-separate Vibrio species. Reference genome data was used to assess the resulting assembly. The workshop follows five stages that include examining reads, assembly, QC, binning, and bin assessment.

The workshop began by examining read length distribution via bioawk and a histogram in R and calculating read N50. Assembly was performed using Flye in metagenome mode via a SLURM batch job. QC involved comparing reference and assembled contig GC content using a custom awk script, then visualising contig GC content against coverage depth in R with point size for contig length and ggrepel labels to help distinguish genomes within the assembly.

Binning was carried out using MetaBAT2, grouping contigs by coverage and composition after preparing a depth file and reordering the assembly to match it. Bin quality was then assessed using CheckM, run via SLURM and an apptainer container.

Overall, the workshop delivered a complete metagenomic assembly workflow from raw reads through assembly, QC, binning, and bin assessment highlighting the added complexity of separating closely related, unevenly abundant genomes in a mixed community.
