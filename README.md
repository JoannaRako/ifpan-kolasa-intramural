# Project title (ifpan-kolasa-intramural)

#### Project logline (technique, organism, tissue type)
Molecular mechanisms of the antidepressant effect of psilocybin using an animal model of treatment-resistant depression. 
FACS (Fluorescence-AcFvated Cell Sorter), 
Rattus norvegicus: Wistar Kyoto (WKY)/Wistar Han (WIS), 
Cells from a selected part of the brain (prefrontal cortex).


## Methods
Through this methodology, we aim to precisely understand how psilocybin impacts small RNA profiles in the context of depression.
---

### *biochemical part*
In the biochemical part of the project, the expression of small RNAs and protein expression at the proteome level in the population of prefrontal cortex neurons were examined.
The neurons were isolated using a cell sorter (FACS, Fluorescence-Activated Cell Sorter), which represented a significant methodological challenge and had not been used in the Institute before.

### *nf-core/smrnaseq*
[Pipeline link](https://nf-co.re/smrnaseq/2.2.4)

This pipeline is built on Nextflow, enabling flexible and reproducible analysis across various computational environments. The nf-core/smrnaseq pipeline is specifically tailored for small RNA sequencing data, making it ideal for our study's requirements.
Core Nextflow options used in this pipeline:
- Revision: 2.2.4
- Profile: Docker
- Protocol: Ilumina
- Genome: [rn6 (UCSC)](https://support.illumina.com/sequencing/sequencing_software/igenome.html)

## Preprocessing
Samplesheet.csv -> prepared in a template format, contains the names and locations of files with raw sequences in fq.gz format, necessary for the functioning of the data processing pipeline.
nf-params.json -> file, contains the location of input and output path


## Analysis
Details of analysis

*notes: all files included in the repo need to be referenced, either in README or other .md files. The analysis has to be fully reproducible, in principle the repo should contain code + description of how to run it while data and results kept outside*

## About this template
Directories:
- _root_ - README.md, *.Rproj, general configuration files, etc.
- raw - raw data
- preprocessing - scripts
- data - useful data, created by scripts/tools/preprocessing
- analysis - analysis source code
- results - output ready to present
