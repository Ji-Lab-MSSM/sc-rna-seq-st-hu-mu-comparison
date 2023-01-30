# sc-rna-seq-st-hu-mu-comparison
Single-Cell and Spatial Transcriptomic Analysis of Human Skin Delineates Intercellular Communication and Pathogenic Cells

This Github contains R markdown files, associated html documents, and Jupyter notebooks.  

SEURAT OBJECTS/DATA CAN BE FOUND HERE:
https://www.dropbox.com/sh/3capqkc6dvng70p/AAB_PrNNgvauiasHWQDxn1Zja?dl=0
# Order of Scripts


## Initial Generation of Objects 
scRNA-seq subpopulation analysis/InitialObjects

### Mouse (mu_int)
1. mu_int_seurat_111320 (Creating mu_int/Integrating mouse data)
2. mu_int_joost_anno_122720 (Adding Joost annotations to mouse data)
3. mu_int_sj_anno_local_122720 (Editing Joost annotations for mouse data)

### Human (ns_int)
1. ns_int_seurat_111420 (Integrating ns_int)
2. ns_int_keep_010923 (Creating ns_int_keep)
3. ns_int_barplot_proportion_120320 (ns_int proportion barplots)
#### Scanorama/Harmony integration comparisons
1. ns_int_harmony_100522 (Integrating ns_int using Harmony)
2. ns_int_scanorama_111123 (Scanorama integration)
3. ns_int_scan24_harm_lisi_122322 (Running LISI on ns_int integrated using Seurat, Harmony, and Scanorama)
4. ns_int_harmony_scanorama_comparison_122322 (LISI comparison b/w Seurat, Harmony, Scanorama)


## Subpopulation Analyses

### IFE cells
scRNA-seq subpopulation analysis/IFE
#### Mouse
1. mu_int_ife_seurat_090922 (Isolating mouse IFE cells)
2. mu_int_ife_filt_seurat_090922 (Filtering mouse IFE cells)
#### Human
1. kc_int_seurat_integration_020520 (Integrating Human KCs)
2. kc_int_filt_seurat_020620 (Filtering human IFE cells)
3. norm_update_seurat_012520 (Generating norm_update)

### Mesenchymal cells
scRNA-seq subpopulation analysis/MES
#### Mouse 
1. mu_int_fib_seurat_102322 (Isolating mouse mesenchymal cells)
#### Human 
1. ns_int_fib_seurat_122920 (Isolating human mesenchymal/fibroblast cells)

### PSU cells
scRNA-seq subpopulation analysis/PSU
#### Mouse
1. mu_int_psu_seurat_070620 (Isolating mouse PSU cells)
#### Human
1. ns_int_psu_noecc_seurat_120920 (Isolating human PSU cells)
2. ns_int_psu_noecc_trad_norm_121020 (Identifying contaminating fibroblasts from human PSU cells)
3. ns_int_psu_filt_seurat_121020 (Filtering human PSU cells)
4. ns_int_psu_ref_seurat_121720 (Removing doublets from human PSU cells)


## Spatial Transcriptomics Analysis
1. n23_p1_seurat_120120 (Processing Spatial Transcriptomics Data)
2. n23_p1_seurat_prediction_merged_confident_CT_020621 (Generating celltype predictions for ST spots using scRNA-seq data)
3. n23_p1_map_predictions_011823 (Mapping scRNA-seq based cell predictions onto Spatial Transcriptomics data)


## Pseudotime Analyses
pseudotime-multiome analyses/pseudotime
### Mouse
1. mu_rna_concat_ag_dpt_12_12_2022 (Calculating pseudotime for mouse cells)
### Human
1. hu_rna_concat_ag_dpt_12_12_2022 (Calculating pseudotime for human cells)
### Combined
1. dpt_AG_pseudo_violin_12_12_2022 (Graphing Violin plots For Diffusion Pseudotime Analysis (+ Difference in Median Bar Plot))


## Multiome Analyses
pseudotime-multiome analyses/multiome
1. s_comb_mo_render


## Disease scRNA-seq
### Mouse
1. mu_psor_pipeline (Isolating Cycling Cells in Mice and Calculating Proportions)
### Human
1. nsc_int_ife_process_1_4_2023 (Processing nsc_int_ife / isolating IFE cells from normal skin samples)
2. pso_cheng_ife_process_1_4_2023 (Processing pso_cheng_ife / Isolating IFE cells from psoriatic skin samples)
3. cheng_ife_process_1_4_2023 (Creating cheng_ife from pso_cheng_ife and nsc_int_ife)
4. cheng_ife_cyc_process_1_4_2023 (Isolating cycling cells from cheng_ife)
5. cheng_prop_anal_1_5_2023 (Human Psoriasis Proportion Analyses)




