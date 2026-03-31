# Molecular Docking Workflow

## Objective
To analyze protein–ligand interaction and evaluate binding affinity using blind docking approaches in CB-Dock2 and AutoDock Tools (ADT).

## Protein and Ligand Details

Protein: Carbonic Anhydrase II (PDB ID: 1CA2)  
Ligand: Acetazolamide (PubChem CID: 1986)

## Tools Used

RCSB PDB, PubChem, UCSF Chimera, Open Babel, CB-Dock2, AutoDock Tools (ADT), PyMOL  

## Workflow

### Protein Preparation
- Removed water molecules and non-standard residues  
- Added hydrogens and Gasteiger charges  
- Saved in .mol2 format  

### Ligand Preparation
- Downloaded in .sdf format  
- Prepared in Chimera  
- Added hydrogens and charges  
- Saved in .mol2 format  

### File Conversion
- Converted files to PDBQT using Open Babel  

## CB-Dock2

- Blind docking with automatic cavity detection  
- Multiple binding cavities identified  
- Best docking score approximately -5.7 kcal/mol  
- Ligand bound within predicted binding pocket  

## AutoDock Tools (ADT)

- Blind docking performed without restricting to a specific active site  
- Total poses generated: 50 (from DLG file)  
- Top 20 conformations selected for analysis  

- Best binding affinity: -5.903 kcal/mol (Mode 1)  
- RMSD for Mode 1: 0.0 Å  

| Mode | Binding Affinity (kcal/mol) | RMSD (Å) |
|------|----------------------------|----------|
| 1    | -5.903                     | 0.0      |
| 2    | -5.447                     | 2.831    |
| 3    | -5.190                     | 3.791    |
| 4    | -5.131                     | 2.841    |
| 5    | -5.086                     | 3.689    |

[Binding Energy Graph](result-graph.jpeg)

[Hydrogen Interactions](image-hydrogen interactions.png)

## Results

- Best binding affinity: -5.903 kcal/mol (~ -5.9 kcal/mol)  
- Total poses generated: 50 (top 20 analyzed)  
- Most conformations cluster around -5.0 kcal/mol  
- Indicates stable and consistent binding  

## Comparison

| Feature        | CB-Dock2       | ADT            |
|---------------|----------------|----------------|
| Docking Type  | Blind docking  | Blind docking  |
| Energy        | ~ -5.7         | -5.903         |
| Conformations | Limited        | 50 generated   |


## Conclusion

Both CB-Dock2 and ADT performed blind docking and produced consistent results in the range of -5 to -6 kcal/mol.  
The best binding pose is -5.903 kcal/mol (~ -5.9 kcal/mol).  
The clustering of conformations around -5.0 kcal/mol indicates stable binding behavior.  
Overall, the ligand shows moderate and reliable interaction with the protein.

## Learning

- Molecular docking workflow  
- Blind docking approaches  
- Protein–ligand interaction analysis  
- Interpretation of docking results using DLG file and energy distribution
