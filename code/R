# You may need SeuratObject v5 if there is error message. Follow the steps introduced here for reproducibility and further analysis: https://github.com/naomihabiblab/BEYOND_DLPFC

library(SeuratDisk)
library(Seurat)
library(ggplot2)

mic_obj <- LoadH5Seurat("/cellular_community/BEYOND_DLPFC_1//2. Cell-type analysis/microglia/data/microglia.h5Seurat")
mic_12_13 <- subset(mic_obj, subset = state %in% c("Mic.12", "Mic.13"))

DimPlot(mic_obj, reduction = "umap", group.by = "state", label = TRUE) + 
  ggtitle("Subpopulations of microglia and immune") + 
  theme_minimal() +
  theme(plot.title = element_text(hjust = 0.5))
