# RVAgene: modeling gene expression dynamics 

### Overview
RVAgene models gene expression dynamics in single-cell or bulk data. Read the paper [here](https://www.biorxiv.org/content/10.1101/2020.11.10.375436v1).

### Requirements
1. Python 3
2. numpy, matplotlib, pytorch, scikit-learn
3. GPU (optional)


### Quickstart
  - Jupyter notebook demo of RVAgene [here](https://github.com/maclean-lab/RVAgene/blob/master/demo.ipynb)
  - Or on the command line
      - python gen_synthetic_data.py <dataset_name> e.g. `python gen_synthetic_data.py demosim`  
      - python train_and_gen.py <dataset_name> e.g. `python train_and_gen.py demosim`

### Contents 
`data` : contains example synthetic gene expression time series data with 6 inherent clusters <br />
`rvagene` : contains code for recurrent variational autoencoder <br />
`train_and_gen.py` : code demonstrating training RVAgene, unsupervised clustering on latent space using K-means and Generating new gene expression data by sampling and decoding points from latent space.  <br />
`gen_synthetic_data.py` : code to generate synthetic data with cluster structure as described in the paper. <br />
`figs` : contains figures generated by the demo code. <br />
`demo.ipynb` : Demonstration on the whole synthetic data generation, RVAgene training, clustering on latent space and new cluster specific data generation process

![alt text](https://github.com/maclean-lab/RVAgene/blob/master/figs/demo.png?raw=true)

### Acknowledgments 
1. Thanks to open source implementation of recurrent VAE  at https://github.com/tejaslodaya/timeseries-clustering-vae
2. Relevant research works as cited in the work.


### Contributors
<a href="https://github.com/maclean-lab/RVAgene/graphs/contributors">
  <img src="https://contributors-img.web.app/image?repo=maclean-lab/RVAgene" />
</a>
