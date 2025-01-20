# Fingerprints

## This project looks at fingerprint similarities between statins with a goal to see which molecules are similar
to one another. Molecular fingerprinting is a technique used to represent molecules as binary vectors or strings,
where each bit or character in the vector or string represents a specific feature of the molecule. This allows for
the efficient comparison of molecules, as the similarity between two molecules can be calculated by comparing their
fingerprints.

## Features
The feature that will be used are smiles which are the string representation of a molecule. These smiles were extracted 
from pubchempy. The compound ID of the statin is utilized to get the smile of the statin from pubchempy. After getting
the smiles of each statin, the smiles are converted to RDKit molecules as they will be needed to get the fingerprints. 
The Tanimoto score is calculated after the fingerprints are obtained.  The Tanimoto score is a measure of similarity
between two fingerprints. It is calculated as the ratio of the number of features that are common to the two fingerprints
to the total number of features in the two fingerprints.
