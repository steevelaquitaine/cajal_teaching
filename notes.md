
file: notes.md 

* title: Computational methods to visualize and analyze high-dimensional neural population and behavioral data.

`abstract`: Modern experimental techniques allow to measure large-scale population activity and behavioral variables and to describe brain information dynamic distribution and to link it to cognition and behavior, both within and across instances of behaviors.

[outcomes] 
At the end of the course students will be able 
- to locate and retrieve open source datasets
- use hypothesis-driven and discovery-driven approaches to visualize and retrieve latent factors from neural activities and to identify the neurons that contribute to them, in mice and monkeys ...
- to understand the advantages and limitations of the most popular techniques (pca, tsne, umap, cebra.ai).

* Open source datasets: 
    * Figshare: https://figshare.com
    * Dandi archive: https://dandiarchive.org/ 

* Datasets:
    * type:
        * real-world time series (calcium, spikes)
        * behavioral labels: reward, 3D kinematics, sensory inputs 
        * time labels:
        * data: spikes, calcium image
    * source:
        * dataset 0:
            * paper: de Vries et al., (2020)
            * ex: https://www.youtube.com/watch?v=XVc_AH42FD4 (53:16)
            * animal model: mouse
            * behavior: natural scene passive viewing (natural movie 1)
            * recording technique: neuropixels, 2P ca-imaging
            * Allen institute
        * dataset 1: 
            * paper: Grossmark, Buzsaki. 2016, Science
            * animal model: mouse
            * behavior: navigation
            * brain activity: Hippocampus, CA1 region
            * recording technique: tetrode recording
            * ex: https://www.youtube.com/watch?v=XVc_AH42FD4 (42:26)
        * dataset 2:
            * download: https://dandiarchive.org/dandiset/000462?search=&pos=1
                * format: NWB
                * size: 6.5 GB
            * animal model: mouse
            * behavior: rewarded navigation
            * recording technique: ca-imaging
            * causal manipulation: DREAD manip.
        * dataset 3:
            * paper: https://elifesciences.org/articles/48198
            * download: https://datadryad.org/stash/dataset/doi:10.5061/dryad.nk98sf7q7
            * animal model: monkey
            * ex: https://www.youtube.com/watch?v=XVc_AH42FD4 (50:40)


* Chosen analytical approaches:
    * hypothesis-testing
        * example: https://www.youtube.com/watch?v=XVc_AH42FD4 (42:43)
    * discovery-driven analyis
        * example: https://www.youtube.com/watch?v=XVc_AH42FD4 (42:43) 

* Chosen techniques:
    * Traditional analyses:
        * TODO: `find existing Allen institute notebook`
    * Unsupervised analyses:
        * CEBRA
            * pros: 
                * visualization but also model with goodness of fit
                * latents are consistent across animals
                * enables real-time (BMI style) decoding (e.g., with a KNN on top)
                    * example: https://www.youtube.com/watch?v=XVc_AH42FD4 (47:55)
                * fast inference
                * works with single trial and across trials
                * interpretability (TO DEFINE)
        * t-SNE
        * piVAE
        * autoLFADS
        * UMAPS

* Chosen software: 
    * Software: CEBRA ? DEEPLABCUT ?
    * Programming language: Python

* Teaching Medium:
    * Jupyter Book ?
    * Develop a codeless light weight webapp to run PCA, t-SNE, UMAP, CEBRA.ai for the course.
        * e.g., https://medium.com/@LeonFedden/comparative-audio-analysis-with-wavenet-mfccs-umap-t-sne-and-pca-cb8237bfce2f 

# Concepts learnt

* Topology


# References

CEBRA, Mathis, Cosyne
https://www.youtube.com/watch?v=XVc_AH42FD4  

Mante et al., Nature 2013
Churchland et al., 2012, Nature, Review
Sadtler Nature 2014
Elsayed cuningham NN, 2017
Urai et al., Nature 2022
Hurwitz 2021, Current opinion in Neuro

Dr. Byron Yu - Dimensionality reduction of large-scale neural recordings - CCCN 2017
https://www.youtube.com/watch?v=KaTnWP1SVpk&list=PLy1BsVH1-Cg8Issbwl-_vjtcfmolAxPrp&index=5



