# Prediction modeling

The activities for the third day were focused on the **tertiary structure prediction** and the **quality assessment** of the models obtained. The main tools used were [AlphaFold 2](https://alphafold.google.com/) and [AlphaFold 3](https://alphafoldserver.com/).

The main objective for this day was to understand the accuracy and compare the quality of known protein structures against the prediction models from AlphaFold.
The AF2 model was run using a [Google Colab](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/AlphaFold2.ipynb) notebook because it has been deprecated in favor of AlphaFold 3. Although it uses ColabFold rather than the original method, the latter is very accurate at simulating the deprecated AF2 model.

## AlphaFold 2 (AF2)
The modeling was performed for the [Gamma-aminobutyric acid receptor subunit rho-1](./AF2/Gamma-aminobutyric%20acid%20receptor%20subunit%20rho-1_P24046.fasta) (GABA receptor). The quality of the model was evaluated using:
- **Swiss-Model**: For MolProbity scores, QMEAN, and Ramachandran plots.
- **SAVES**: Specifically using ERRAT and VERIFY 3D for quality control.

The detailed analysis and results can be found in the [AF2 summary](./AF2/summary/summary.md).

## AlphaFold 3 (AF3)
The [Early growth response protein 1 (EGR1)](./AF3/EGR1_P18146_full.fasta) was modeled in two versions:
- **Full Sequence**: To observe the disordered regions.
- **Trimmed Sequence**: Focusing on the structured DNA-binding domain (residues 335-423).

For AF3, the quality assessment was primarily done through [Swiss-Model](./AF3/swiss_model/) due to the compatibility of the `.cif` output format with the MolProbity tools integrated into it.

The detailed comparison between the models is available in the [AF3 summary](./AF3/summary/summary.md).

## Quality Assessment Tools
To ensure the reliability of the predicted structures, several metrics were used:
- **MolProbity Score**: Combines various geometric features to estimate resolution-like quality.
- **QMEAN**: A global and local estimator of geometrical properties (0 to 1 scale).
- **Ramachandran Plot**: Analysis of $\phi$ and $\psi$ angles to identify stereochemical outliers.
- **SAVES (ERRAT/Verify 3D)**: Additional validation for protein environment and residue distribution.

<br>
<br>
<br>
<br>
<br>

Full course in: https://eead-csic-compbio.github.io/bioinformatica_estructural/
