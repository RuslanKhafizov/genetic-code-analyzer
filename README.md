# Interactive explorer of genetic code symmetries.

An interactive tool demonstrating the division of all 24 genetic code calligrams into 6 distinct orbits under Rumer-related transformations.
Simply open the `index.html` file in a modern web browser or https://ruslankhafizov.github.io/genetic-code-analyzer

## Scientific Background and Key Concepts

The tool visualizes and allows interaction with the following core ideas:

1.  **Rumer's Octets**
    *   As first noted by [Y. B. Rumer](https://www.prometeus.nsc.ru/science/schools/rumer/works/1968.ssi), the 16 "columns" (XY-boxes, defined by the first two nucleotides of a codon) in the standard genetic code table can be divided into two groups of eight:
        *   **Octet I:** XY-boxes where all four codons (XYN) code for the same amino acid (4-fold degeneracy).
        *   **Octet II:** The remaining XY-boxes without such complete degeneracy.
    *   This tool dynamically determines the Octet I/II assignment for the standard genetic code.

2.  **Rumer's R-Transformation**
    *   Y. B. Rumer also identified a symmetry transformation **R = (T↔G, C↔A)** (or U↔G, C↔A in RNA) that interconverts XY-boxes between Octet I and Octet II.

3.  **Codograms and Code Representations**
    *   The concept of a **codogram** was introduced by [Vladimir Shcherbak and Maxim Makukov](https://arxiv.org/pdf/1707.03382) as a 4x4 visual representation of the genetic code, where cells are colored based on their Octet I/II assignment.
    *   There are 24 possible "homogeneous representations" when ordering the four nucleotides on the axes of the codogram.

4.  **Simply-Connected Codograms and the {E, R, R1, R2} Transformation Group**
    *   [Alexander D. Panov and Felix P. Filatov](https://www.sociostudies.org/almanac/articles/are_the_strange_information_structures_of_the_genetic_code_an_accident_or_an_artifact) identified four "simply-connected" codograms where Octet I and II regions are continuous.
    *   They showed these are closed under the transformations:
        *   **R** (full Rumer): U↔G, C↔A
        *   **R1** ("purine" Rumer transformation): U↔G
        *   **R2** ("pyrimidine" Rumer transformation): C↔A
        *   **E** (identity)
    *   These transformations form the Klein four-group (V₄).

5.  **Codogram Orbits**
    *   Ruslan Khafizov, the developer of this tool, established that all 24 homogeneous codograms are divided by the {E, R, R1, R2} transformation group into **6 disjoint orbits**. Each orbit contains 4 codograms:
        *   `{TCAG, GACT, GCAT, TACG}`
        *   `{TCGA, GATC, GCTA, TAGC}`
        *   `{CTAG, AGCT, CGAT, ATCG}`
        *   `{CTGA, AGTC, CGTA, ATGC}`
        *   `{TGCA, GTAC, TGAC, GTCA}`
        *   `{ACGT, CATG, ACTG, CAGT}`

## Physico-Chemical and Structural Consequences of Rumer Transformations Analyzed

1.  **Conservation of Amino/Keto Type of XY-boxes:**
    All Rumer transformations (R, R1, R2) preserve the amino-group (A, C) or keto-group (U, G) nature of each nucleotide. Consequently, the classification of XY-boxes based on the amino/keto composition of their nucleotide positions (e.g., Amino-Keto, Keto-Keto) is invariant under the entire Rumer transformation group.

2.  **Purine ↔ Pyrimidine Transformations (Transversions):**
    The full R-transformation (U↔G, C↔A) always acts as a transversion for both nucleotides in an XY-box, changing a purine to a pyrimidine and vice versa. The "half" transformations R1 (U↔G) and R2 (C↔A) also perform transversions but only for the nucleotides they affect.

3.  **Regular Changes in Nucleotide Bonding "Strength":**
    Rumer transformations lead to predictable changes in nucleotide "strength" (H-bonds: Weak W – A/U; Strong S – G/C). The full R-transformation always changes the strength of each nucleotide in an XY-box (W↔S); R1 and R2 alter strength only for their target pairs.

## Features

This tool allows users to:

*   Visualize all 6 codogram orbits.
*   Display the 4 codograms within each orbit, corresponding to the E, R1(E), R2(E), and R(E) transformations of the orbit's representative.
*   Observe the Octet I (black cells) and Octet II (white cells) structure for the standard genetic code.
*   Interactively apply R, R1, and R2 transformations to the currently displayed orbit and see the resulting codogram structures and nucleotide order changes.
*   Highlight nucleotides involved in the selected transformation on the axes and titles of the codograms.

## Author
Ruslan Khafizov
*   **Email:** <a href="mailto:jhgf10@gmail.com">jhgf10@gmail.com</a>
*   **YouTube:** <a href="https://www.youtube.com/@ruslankhafizov251">@ruslankhafizov251</a>
*   **Facebook:** <a href="https://www.facebook.com/russopirato/">Profile</a>

## License
MIT License
