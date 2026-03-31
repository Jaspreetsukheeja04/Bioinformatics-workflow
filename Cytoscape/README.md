# Cytoscape Workflow for PPI Network Analysis

## Objective
To analyze protein–protein interaction (PPI) networks using gene expression data and identify key hub genes using Cytoscape.


## Tools Used

STRING database, Cytoscape, Microsoft Excel  

## Input Data

- Gene list obtained from RNA-seq analysis  
- Genes categorized as upregulated and downregulated based on log2 fold change  

## Workflow

### 1. Gene List Preparation
- Prepared gene list in Excel  
- Calculated log2 fold change values  
- Classified genes into upregulated and downregulated groups  

### 2. STRING Database Analysis
- Uploaded gene list to STRING database  
- Generated PPI network  
- Selected appropriate organism  
- Exported network as TSV file  

### 3. Network Import in Cytoscape
- Opened Cytoscape  
- Imported TSV network file  
- Network visualized in Cytoscape workspace  

### 4. Network Visualization
- Used Style panel for customization  
- Applied node color coding:
  - Red for upregulated genes  
  - Green for downregulated genes  
- Adjusted node size and edge properties  

### 5. Network Analysis
- Used Network Analyzer tool  
- Calculated topological parameters  
- Sorted nodes based on degree  
- Identified hub genes (high-degree nodes)  

### 6. Hub Gene Identification
- Selected top nodes based on degree  
- Highlighted hub genes using different color and shape  
- Used circular layout for better visualization  

### 7. Attribute Mapping
- Imported gene expression data (log2 fold change)  
- Applied continuous mapping  
- Set value range from -1 to +1  
- Visualized expression levels using color gradients  

### 8. Export Results
- Exported network images in PNG format  
- Saved:
  - Complete network  
  - Hub gene network  

## Results

- PPI network successfully generated from gene list  
- Hub genes identified based on node degree  
- Clear distinction between upregulated and downregulated genes  
- Network visualization improved using attribute mapping  

## Conclusion

Cytoscape enabled effective visualization and analysis of PPI networks.  
Hub genes were identified, providing insights into key biological interactions.  
The workflow demonstrates how gene expression data can be integrated with network biology tools for meaningful interpretation.

## Learning

- PPI network construction and analysis  
- Use of STRING database and Cytoscape  
- Network topology analysis and hub gene identification  
- Data visualization using attribute mapping
