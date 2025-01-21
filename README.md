## Fingerprints
This project looks at fingerprint similarities between statins with a goal to see which molecules are similar
to one another. Molecular fingerprinting is a technique used to represent molecules as binary vectors or strings,
where each bit or character in the vector or string represents a specific feature of the molecule. This allows for
the efficient comparison of molecules, as the similarity between two molecules can be calculated by comparing their
fingerprints.

### Features
The feature that will be used are smiles which are the string representation of a molecule. These smiles were extracted 
from pubchempy. The compound ID of the statin is utilized to get the smile of the statin from pubchempy. After getting
the smiles of each statin, the smiles are converted to RDKit molecules as they will be needed to get the fingerprints. 
The Tanimoto score is calculated after the fingerprints are obtained.  The Tanimoto score is a measure of similarity
between two fingerprints. It is calculated as the ratio of the number of features that are common to the two fingerprints
to the total number of features in the two fingerprints.

### Dataset
The technical information about the statins was imported from pubchempy. The statins that are utilized are Simvastatin,
Pravastatin, Atorvastatin,and Fluvastatin.

## Requirements
- **Libraries**
  - **PCP**
  - **RdKit**

## Results
The similarity shown below is the one that was the greatest than the other similarity values hence a greater Tanimato
Similarity shows a higher similarity.

1. Simvastatin
Simvastatin and Pravastatin shows a greater degree of similarity with a tanimoto score of 0.872 which is higher tanimoto similarity than other statins.

2. Pravastatin
As mentioned previously, Pravastatin and Simvastatin shows a higher similarity with a tanimoto score 0.872.

3. Atorvastatin
Atorvastatin and Fluvastatin have a greater similarity with a tanimoto score of is 0.522.

4. Fluvastatin
As mentioned previously, Fluvastatin and Atorvastatin have a higher similarity in comparison to other statins with a tanimoto score of 0.522.

## Future Work
- It would have been better if I displayed the closest match of each statin in a calculated way but I just did it manually as I do see the values.
- Integrate this logic with a web application for better interactivity. 
