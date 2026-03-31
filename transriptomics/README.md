# Transcriptomics Workflow (RNA-seq Analysis)

## Objective
To perform RNA-seq data analysis including quality control, preprocessing, and alignment using the Galaxy platform.

## Tools Used

NCBI SRA, Galaxy Platform, FastQC, MultiQC, Trim Galore, HISAT2  

## Input Data

- RNA-seq dataset retrieved from NCBI Sequence Read Archive (SRA)  
- Paired-end sequencing data converted to FASTQ format  

## Workflow

### 1. Data Retrieval
- RNA-seq data downloaded from NCBI SRA  
- Converted into FASTQ format for analysis  

### 2. Quality Control (Initial)
- Performed FastQC on forward and reverse reads  
- Assessed sequence quality, GC content, and adapter contamination  

---

### 3. Quality Summary
- Used MultiQC to combine FastQC reports  
- Evaluated overall data quality across samples  

### 4. Data Preprocessing
- Applied Trim Galore on FASTQ files  
- Removed adapter sequences  
- Trimmed low-quality bases  
- Standardized reads to Sanger format  

### 5. Post-trimming Quality Check
- Re-ran FastQC after trimming  
- Confirmed improvement in read quality  

---

### 6. Read Alignment
- Performed alignment using HISAT2  
- Mapped reads to reference genome  
- Generated alignment files for downstream analysis  

## Results

- Initial FastQC showed variation in sequence quality  
- Trim Galore improved read quality without significant data loss  
- Post-trimming FastQC showed improved Phred scores  
- Majority of reads shifted toward acceptable to high-quality range  
- HISAT2 achieved efficient and reliable alignment  

## Quality Interpretation

- Phred score ≥ 30 indicates high-quality bases  
- Phred score 20–30 indicates acceptable quality  
- Phred score < 20 indicates low-quality bases  

## Conclusion

RNA-seq workflow successfully improved data quality and achieved accurate read alignment.  
Preprocessing steps significantly enhanced the reliability of downstream analysis.  
The workflow demonstrates the importance of quality control in transcriptomic studies.

## Learning

- RNA-seq data preprocessing and quality control  
- Use of Galaxy platform for bioinformatics analysis  
- Interpretation of FastQC and MultiQC reports  
- Read alignment using HISAT2
