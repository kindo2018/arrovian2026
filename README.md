
# Arrovian Possibility: Sheaf-Theoretic Navigation
This repository contains the Prolog implementation and computational experiment data for the paper:  
**"Holonomic Information Management: Sheaf-Theoretic Navigation of Arrovian Possibility"** (JSAI-IS AiBiz 2026).


## 1. Overview
This project provides a novel framework to formalize organizational decision-making as a **patching problem** of local preferences within a **sheaf**. While Arrow's Impossibility Theorem identifies topological obstructions to global consistency , this methodology identifies and excises these "singularities" to restore **Arrovian Possibility** within maximal consistent domains.

### Key Features
* **Sheaf-Theoretic Formalization**: Modeling preference aggregation as a section-patching problem over a simplicial complex.
* **Singularity Excision**: Systematically identifying and removing intransitive triples (topological obstructions) using Alexander duality.
* **Prolog Implementation**: A rigorous, recursive functional generator for exhaustive search and verification of maximal consistent regimes. So, the axiomatic theories of social choice can be intuitively described as a logical formula and is well-suited for exhaustive search..
* **Prevalence Analysis**: Quantitative mapping showing that consistent domains cover 85% to 97% of the total preference space.



## 2. Theoretical Background
The framework uses **Abstract Managerial Information Schemata (AMIS)** to bridge the gap between social choice axioms and algebraic topology:
* **IIA (Independence)**: Guaranteed by binary decomposition.
* **Transitivity**: Formalized as the sheaf consistency condition.
* **Holonomy**: Detecting systemic failures via parallel transport around cycles in the organizational structure.

## 3. Repository Structure
* `/prolog`: Contains the core recursive functional generator (main.pl) for generating binary aggregation rules and obstruction collecting, and helper programs (lib2025.pl). And the profile-based aggregation rule generator (arrow2025.pl) is also included.
* `/data`: Results for various cases $(n, m)$, including maximal possibility rules, minimal cuts (obstructions).
* `/docs`: Examples of maximal governance rules and their structural properties.

## 4. How to Run the Experiments
The code is implemented in **Prolog**. To reproduce the results shown in the paper:

1. Install a Prolog interpreter (e.g., SWI-Prolog).
2. Load the main generator:
   ```prolog
   ?- [main_generator].
   ```
3. Run the search for a specific configuration (e.g., $n=2, m=3$):
   ```prolog
   ?- find_maximal_consistent_domains(2, 3, Results).
   ```

## 5. Key Results
Our experiments reveal that topological "No-go" zones are concentrated in sparse singularities, restoring practical possibility for information management.
* **Prevalence Ratios**:
  * $(n, m) = (2, 3)$: 94.4% 
  * $(n, m) = (2, 4)$: 87.5% 
  * $(n, m) = (2, 5)$: 85.0% 
* **Symmetry**: Odd-numbered groups ($n=3$) can achieve perfect fairness (inequality index $1/3$), unlike even-numbered groups.

## 6. Citation
If you use this code or framework in your research, please cite:
```bibtex
@inproceedings{Indo2026,
  author    = {Kenryo Indo},
  title     = {Holonomic Information Management: Sheaf-Theoretic Navigation of Arrovian Possibility},
  booktitle = {Proceedings of JSAI-IS AiBiz 2026},
  publisher = {Springer},
  year      = {2026}
}
```
## Notes & Ackowledgements
This work will be primarily presented at JSAI-IS AI Biz 2026 (June 2026, Takasaki, Japan). Preliminary findings related to certain experimental results were previously shared during the Decision Making session at the 2026 Spring Conference of the Operations Research Society of Japan (ORSJ), held at Reitaku University from March 4th to 6th, 2026. The core codebase for those experiments remains substantially consistent with this repository (see https://github.com/kindo2018/or2026).

---
