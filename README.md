# Visualizations of Genotype Datasets

This repository contains the visualizations of 1000 Genomes dataset ([1000 Genomes Project Consortium](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3498066/)) and the modern Eurasian population dataset ([Lamnidis et al.](https://www.nature.com/articles/s41467-018-07483-5)). The dimensional reduction techniques used include PCA, t-SNE, UMAP, and Adversarial Autoencoders ([Makhzani et al.](https://arxiv.org/pdf/1511.05644.pdf))

All visualizations can be founded in the form of interactive htmls in the `htmls` folder. The interactive htmls let you pan, zoom, hover on data points, and also hide data of particular labels by clicking on the legend. 

We also hand pick some visualizations and display them as static images below.

## 1000 Genomes

For reference, [Diaz-Papkovich et al.](https://journals.plos.org/plosgenetics/article?id=10.1371/journal.pgen.1008432) have applied PCA, t-SNE, and UMAP to the 1000 Genomes dataset. The following figure is the first figure in the paper

![Diaz-Papkovich.png](imgs/Diaz-Papkovich.png)

**A** corresponds to PCA outputs. **B** corresponds to t-SNE outputs. **C** corresponds to UMAP outputs. **D** correponds to the outputs of first applying PCA to reduce the dimension down to 15 and then applying UMAP

Our results are below:

- PCA

![1kgenome_2pcs.png](imgs/1kgenome_2pcs.png)

- t-SNE

![1kgenome_tsne_p30.png](imgs/1kgenome_tsne_p30.png)

- UMAP

![1kgenome_umap_nn10_md0.5.png](imgs/1kgenome_umap_nn10_md0.5.png)

- UMAP on 15 PCs

![1kgenome_15pcs-umap_nn10_md0.5.png](imgs/1kgenome_15pcs-umap_nn10_md0.5.png)

- Vanilla Adversarial Autoencoders

![1k_vanilla_lr0.0005_bs128.png](imgs/1k_vanilla_lr0.0005_bs128.png)

- Adversarial Autoencoders with Cluster Heads

![1k_dim_20_lr0.0005_bs32_std0.5.png](imgs/1k_dim_20_lr0.0005_bs32_std0.5.png)

We haven't managed to exactly reproduce the results from Diaz-Papkovich et al; we're working on it. 

And feel free to explore the visualizations further using the interactive htmls that can be founded in the `htmls` folder

## Modern Eurasian population

For reference, [Lamnidis et al.](https://www.nature.com/articles/s41467-018-07483-5) have applied PCA to this dataset:

![Lamnidis.png](imgs/Lamnidis.png)

Our results are below:

- PCA

![eurasia_2pcs.png](imgs/eurasia_2pcs.png)

- t-SNE

![eurasia_tsne_p30.png](imgs/eurasia_tsne_p30.png)

- UMAP

![eurasia_umap_nn30_md0.5.png](imgs/eurasia_umap_nn30_md0.5.png)

- UMAP on 15 PCs

![eurasia_15pcs-umap_nn15_md0.5.png](imgs/eurasia_15pcs-umap_nn15_md0.5.png)

- Vanilla Adversarial Autoencoders

![eurasia_vanilla_lr0.0005_bs128.png](imgs/eurasia_vanilla_lr0.0005_bs128.png)

- Adversarial Autoencoders with Cluster Heads

![eurasia_dim_20_lr0.0001_bs32_std0.5.png](imgs/eurasia_dim_20_lr0.0001_bs32_std0.5.png)








