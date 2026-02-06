# LCE Proofs

Mathematical proofs relating TFCE (Threshold-Free Cluster Enhancement) and LCE (Local Cluster Enhancement) significance in neuroimaging statistical analysis.

## Project Structure

- `clusterproof/proof.tex` - Main LaTeX document containing theorems and proofs
- `clusterproof/proof.pdf` - Compiled PDF output
- `TFCE_Finds_Cluster_Errors (6).pdf` - Reference document

## Key Concepts

- **TFCE**: Threshold-Free Cluster Enhancement - a statistical method for neuroimaging
- **LCE**: Local Cluster Enhancement - a related statistical method
- **Superthreshold clusters**: Connected regions where test statistics exceed a threshold $h_0$
- **Excursion sets**: $\mathcal{E}(h) = \{w \in \mathcal{B} : T_w \geq h\}$

## Working with This Repository

### LaTeX Compilation

Compile the proof document:
```bash
cd clusterproof && pdflatex proof.tex
```

### Mathematical Notation

- $R, R'$ - Clusters (regions)
- $\mathcal{B}$ - Brain mask / search region
- $T_v$ - Test statistic at voxel $v$
- $C_v(h)$ - Connected component containing voxel $v$ at threshold $h$
- $S_v$ - TFCE statistic at voxel $v$
- $t^*_\mathcal{B}$ - Significance threshold

### Comments

Author comments use the `\sdcom{}` macro (displays in red).

## Guidelines

- Maintain mathematical rigor in all proofs
- Use standard LaTeX theorem environments (`theorem`, `lemma`, `corollary`, `remark`)
- Keep notation consistent with existing definitions
- When editing proofs, preserve the logical flow and ensure all lemmas are properly referenced
