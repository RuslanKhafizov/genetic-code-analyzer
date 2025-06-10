# genetic-code-analyzer
An interactive tool demonstrating the division of all 24 genetic code calligrams into 6 distinct orbits under Rumer-related transformations.
# Interactive Rumer Orbit Explorer

This interactive web tool is designed for visualizing, exploring, and analyzing the structural and mathematical symmetries inherent in the genetic code. It focuses on the concepts first proposed by **Yuri Borisovich Rumer** and subsequent developments related to calligram (or "codogram") transformations and orbits.

The application is implemented فيلمstrip (using vanilla JavaScript without external frameworks like React for this particular version) and renders directly in the browser.

## Scientific Background and Key Concepts

The tool visualizes and allows interaction with the following core ideas:

1.  **Rumer's Octets:**
    *   As first noted by **Y.B. Rumer**, the 16 "columns" (XY-boxes, defined by the first two nucleotides of a codon) in the standard genetic code table can be divided into two groups of eight:
        *   **Octet I:** XY-boxes where all four codons (XYN) code for the same amino acid (4-fold degeneracy).
        *   **Octet II:** The remaining XY-boxes without such complete degeneracy.
    *   This tool dynamically determines Octet I/II assignment for the standard genetic code.

2.  **Rumer's R-Transformation:**
    *   **Y.B. Rumer** also identified a symmetry transformation **R = (T↔G, C↔A)** (or U↔G, C↔A in RNA) that interconverts XY-boxes between Octet I and Octet II.

3.  **Codograms (Calligrams) and Code Representations:**
    *   The concept of a **codogram** (often referred to as a calligram) was introduced by **Vladimir I. Shcherbak** and **Maxim A. Makukov** (see <a href="https://arxiv.org/pdf/1707.03382" target="_blank" rel="noopener noreferrer">Shcherbak & Makukov, 2013 / arXiv:1707.03382</a>) as a 4x4 visual representation of the genetic code, where cells are colored based on their Octet I/II assignment.
    *   There are 24 possible "homogeneous representations" when ordering the four nucleotides on the axes of the codogram.

4.  **Simply-Connected Codograms and the {E, R, R1, R2} Transformation Group:**
    *   **Alexander D. Panov** (see <a href="http://dec1.sinp.msu.ru/~panov" target="_blank" rel="noopener noreferrer">personal page</a>, <a href="https://www.socionauki.ru/news/3562368" target="_blank" rel="noopener noreferrer">publication</a>) and **Felix P. Filatov** identified four "simply-connected" codograms where Octet I and II regions are continuous.
    *   They showed these are closed under the transformations:
        *   **R** (full Rumer): U↔G, C↔A
        *   **R1** ("purine" Rumer transformation): U↔G
        *   **R2** ("pyrimidine" Rumer transformation): C↔A
        *   **E** (identity)
    *   These form the Klein four-group (V₄).

5.  **Codogram Orbits (Research by Ruslan Khafizov):**
    *   **Ruslan Khafizov** (contact: <a href="mailto:jhgf10@gmail.com">jhgf10@gmail.com</a>), the developer of this tool, established that all 24 homogeneous codograms are divided into **6 disjoint orbits** by the {E, R, R1, R2} transformation group. Each orbit contains 4 codograms:
        *   {TCAG, GACT, GCAT, TACG}
        *   {TCGA, GATC, GCTA, TAGC}
        *   {CTAG, AGCT, CGAT, ATCG}
        *   {CTGA, AGTC, CGTA, ATGC}
        *   {TGCA, GTAC, TGAC, GTCA}
        *   {ACGT, CATG, ACTG, CAGT}

## Features

This tool allows users to:

*   Visualize all 6 codogram orbits.
*   Display the 4 codograms within each orbit, corresponding to the E, R1(E), R2(E), and R(E) transformations of the orbit's representative.
*   Observe the Octet I (black cells) and Octet II (white cells) structure for the standard genetic code.
*   Interactively apply R, R1, and R2 transformations to the currently displayed orbit and see the resulting codogram structures and nucleotide order changes.
*   Highlight nucleotides involved in the selected transformation on the axes and titles of the codograms.

## How to Use

Simply open the `index.html` (or `Khafizov_Ruslan (1).html` if you haven't renamed it) file in a modern web browser.
Alternatively, if deployed via GitHub Pages, access it via the provided URL.

## Technologies Used

*   Vanilla JavaScript (ECMAScript 6+)
*   HTML5
*   CSS3

## Author

*   **Ruslan Khafizov**
    *   Email: <a href="mailto:jhgf10@gmail.com">jhgf10@gmail.com</a>
    *   GitHub: https://github.com/RuslanKhafizov

## Acknowledgements

This work builds upon the foundational concepts and research of:

*   **Yuri B. Rumer** (Octets, R-transformation)
*   **Vladimir I. Shcherbak** & **Maxim A. Makukov** (Calligrams/Codograms - <a href="https://arxiv.org/pdf/1707.03382" target="_blank" rel="noopener noreferrer">arXiv:1707.03382</a>)
*   **Alexander D. Panov** & **Felix P. Filatov** (Simply-connected calligrams, {E,R,R1,R2} group closure for these - <a href="http://dec1.sinp.msu.ru/~panov" target="_blank" rel="noopener noreferrer">A.D. Panov's page</a>, <a href="https://www.socionauki.ru/news/3562368" target="_blank" rel="noopener noreferrer">related publication</a>)

Deep respect is expressed for their pioneering contributions.
