# scCrossEvo
Single Cell Cross Species Evolutianary Pipeline

A computational pipeline for cross-species comparative single-cell transcriptomics across 700 million years of evolutionary divergence (Hydra vulgaris vs. Nematostella vectensis). This workflow evaluates cell-type evolutionary dynamics by integrating a 1:1 orthology backbone with a Paralog-Weighted Principal Component Analysis (WPCA) and a single-cell-adapted Transcriptome Age Index (TAI*).

Overview

Standard single-cell batch integration algorithms (e.g., Harmony, Seurat CCA, scVI) treat evolutionary divergence as technical batch noise, forcing macroevolutionary differences to collapse into shared manifold space.

This repository provides an alternative framework:
Unforced Comparative Manifolds: Builds an anchored 1:1 orthology backbone across species, applying Weighted PCA (WPCA) scaled by gene family dynamism to retain authentic evolutionary divergence without artificial clustering collapse. 

TAI*(Transcriptome Innovation Index): Extends classical phylotranscriptomic age indexing to single-cell data by incorporating multigene family expansion dynamics (log2(1 +copies) and implementing an expression cap on single-gene transcriptomic monopolies. 

Biological Validation: Resolves classical phylotranscriptomic artifacts, demonstrating that cnidarian cell-type novelty is governed by two distinct evolutionary strategies: Gene Family Expansion and Orphan Monoculture. 
