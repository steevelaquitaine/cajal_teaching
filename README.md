# CAJAL 2024

Author and instructor: steeve.laquitaine@epfl.ch; laquitainesteeve@gmail.com  
For the Cajal advanced training course, 2024, Bordeaux

## Abstract

**Project**: "Computational analytical methods to link high-dimensional neuronal population and behavioral data"

**Instructor**: Steeve Laquitaine, PhD (Swiss Federal Institute of Technology, Switzerland)

Modern technical innovations now allow experimentalists to measure and manipulate the dynamic distributed activity of large populations of neurons in behaving animals. With recent progress in machine learning, they now also have the capability to link neural population activity with behavior in real-time, across days, across a wide range of tasks and animals. The massive datasets generated have stimulated the rise of an Open Science framework to store, share and accelerate data and analyses within the Neuroscience community, in a standardized and reproducible manner. At the end of the course students will be able to locate, retrieve datasets made available by the research community and to share their own with the community. They will know how to use state-of-the-art modeling and visualisation techniques, via discovery-driven and hypothesis-driven approaches, to identify factors that explain joint changes in neural activity and behavior in 2P ca-imaging, extracellular electrophysiological recording experiments, across species. They will learn to identify the neurons that contribute to these variations. They will understand the advantages and limitations of traditional and popular modern techniques and know how to use them to arbitrate between techniques.

**Main outcomes**:

  * Know how to use the Allen Institute SDK, browse the Dandi archive, FigShare, dataryad to retrieve and share standardized, repropducible datasets and code
  * How to analyze (approaches) and characterize (metrics) high-dimensional neural data
  * Understand the advantages and limitations of the most popular analytical techniques
  * Know how to implement and rule out models that link neuronal activity to behavior (model selection via decoding, goodness-of-fit, consistency, robustness).

**Methodology**: 

- Analysis of neuropixels recordings and ca-imaging of cortical activity in mice viewing natural scenes (de Vries et al., 2020, Allen Institute dataset), 
- Analysis of tetrode recordings of Hippocampus activity in mice during virtual navigation (Grossmark, Buzsaki, Science, 2016), 
- Analysis of DREAD manipulation and ca-imaging of cortical activity in mice during reward-based navigation (Krishnan et al., Nat Commun, 2022)
- Analysis of 100-electrode array recording of monkeys' motor cortical activity during motor reaching (Chowdhury et al., elife, 2020).
- Traditional and state-of-the art machine learning-based dimensionality reduction techniques, topological data analysis of neural manifolds
- Programming in Python, low-code for beginners, full code available for tuning
- Programming in Google Colab, on Laptop

## **0. Prerequisites (DAY 1)**

**Notebooks**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/0_Prerequisites.ipynb).

## **1. Theory: From neural tuning to manifolds**

**Learning outcomes**:

* Know <u>what is a manifold</u> and what it is not.
* Know what is an <u>entangled manifold</u> and how to <u>disentangle</u> it.
* Know how to <u>link individual neurons' tuning functions</u> and <u> population manifolds</u> in the absence of noise (simplification). 
* Recognize the <u>different types of underlying neural codes</u> ("splitter", "lumper")

**Readings**: Kriegeskorte, N., & Wei, X. X. (2021). Neural tuning and representational geometry. Nature Reviews Neuroscience, 22(11), 703-718.

**Python prerequisites**

* installing and importing libraries
* using functions
* plotting with matplotlib library

**Notebooks**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/1_Tuning_to_Manifolds.ipynb).
  
## **2. Theory: Manifold dimensionality**

**Learning outcome**:  

  * Know what manifold dimensionality is and why it matters.
  * Know the factors that determine the manifold's dimensionality and how.

**Readings**:

  * Wärnberg and Kumar, “Perturbing Low Dimensional Activity Manifolds in Spiking Neuronal Networks.”
  * Rigotti, M., Barak, O., Warden, M. R., Wang, X. J., Daw, N. D., Miller, E. K., & Fusi, S. (2013). The importance of mixed selectivity in complex cognitive tasks. Nature, 497(7451), 585-590.
  * Cunningham, J. P., & Yu, B. M. (2014). Dimensionality reduction for large-scale neural recordings. Nature neuroscience, 17(11), 1500-1509.
  
**Notebooks**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/2_Manifold_dimensionality.ipynb).

## **3. Hands-on: PCA-based manifolds**

**Learning outcomes:**  
  * Know how to <u>compute manifolds for large populations of neurons</u>, using a simple machine learning technique, `PCA`.
  * Know what is the <u>representational geometry</u> framework.
  * Know how the manifold geometry depends on its individual neurons' tuning functions. 
  * Know how to <u>measure the dimensionality of neural manifolds</u>, with `PCA`.

**Readings**: Kriegeskorte, N., & Wei, X. X. (2021). Neural tuning and representational geometry. Nature Reviews Neuroscience, 22(11), 703-718.

**Python prerequisites**

* installing and importing libraries
* using functions
* plotting with matplotlib library
  
**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/3_PCA_based_manifolds.ipynb).



## **4. Hands-on: Cebra beats them all**

**Learning outcomes:**

  * Know how to <u>compute manifolds</u> from large neuron populations with `state-of-the-art (SOTA) machine learning techniques`.
  * Know what <u>latent variable models</u> are.
  * Know what <u>identifiability</u> is and why it matters.
  * Know how to <u>benchmark SOTA machine learning techniques</u> on a synthetic dataset, using a `linear reconstruction R-squared`.
    
**Method**:

  * With the students, we study the paper section on the generation of the synthetic dataset, describe the design and its objectives in class.

**Readings:** 

* Cunningham, J. P., & Yu, B. M. (2014). Dimensionality reduction for large-scale neural recordings. Nature neuroscience, 17(11), 1500-1509.
* Gokcen, E. (2023). Disentangling communication across populations of neurons (Doctoral dissertation, Carnegie Mellon Univers
* Hurwitz, C., Kudryashova, N., Onken, A., & Hennig, M. H. (2021). Building population models for large-scale neural recordings: Opportunities and pitfalls. Current opinion in neurobiology, 70, 64-73.
* Zhou, D., & Wei, X. X. (2020). Learning identifiable and interpretable latent models of high-dimensional neural activity using pi-VAE. Advances in Neural Information Processing Systems, 33, 7234-7247.
* Schneider, S., Lee, J. H., & Mathis, M. W. (2023). Learnable latent embeddings for joint behavioural and neural analysis. Nature, 617(7960), 360-368.
* Altan, E., Solla, S. A., Miller, L. E., & Perreault, E. J. (2021). Estimating the dimensionality of the manifold underlying multi-electrode neural recordings. PLoS computational biology, 17(11), e1008591.

**Python prerequisites**

* installing and importing `libraries`
* using `functions`
* plotting with `matplotlib` library
* basics of `scikit-learn` software for machine learning
* basics of `Keras` for Deep Learning

**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/4_Cebra_beats_them_all.ipynb).



## **5. Hands-on: movement neural manifold in primate's S1 (InfoNCE loss)**

**Learning outcomes:**
  * Know how to <u>use CEBRA to compute neural manifolds</u> from the monkey's primary somatosensory cortex (S1), for variables of a reaching task.
  * Know how to train the model with the `standard infoNCE loss`.

**Method:**
  * Students study the paper section on the task, describe its design and objectives.

**Readings**:

* Schneider, S., Lee, J. H., & Mathis, M. W. (2023). Learnable latent embeddings for joint behavioural and neural analysis. Nature, 617(7960), 360-368. Shown in Fig. 3, Extended Data Fig. 8

**Python prerequisites**:

* installing and importing `libraries`
* plotting with `matplotlib` library
  
**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/5_handson_movement_manifold_primate_S1_infoNCE_loss.ipynb).



## **6. Hands-on: movement neural manifold in primate's S1 (MSE loss)**

**Learning outcomes:**
  * Know how to <u>train CEBRA to compute neural manifolds</u> by minimizing the `mean squared error (MSE) loss`.
  * Know why the loss used matters.

**Method:**

  * Students study the paper section on the task, describe its design and objectives.

**Readings**:

* Schneider, S., Lee, J. H., & Mathis, M. W. (2023). Learnable latent embeddings for joint behavioural and neural analysis. Nature, 617(7960), 360-368. Shown in Fig. 3, Extended Data Fig. 8

**Python prerequisites**:

* installing and importing `libraries`
* plotting with `matplotlib` library
  
**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/6_handson_movement_neural_manifolds_primate_S1_mse_loss.ipynb).




## **7. Hands-on: navigation neural manifold with discovery analysis in rat's HPC**

**Learning outcomes:**

  * know how to perform a <u>discovery-driven analysis</u> to <u>explore the neural manifolds</u> with `CEBRA-Time`.
  * know how to <u>save a trained model</u> for later re-use.

**Method:**

  * Students study the paper section on the task, describe its design and objectives.

**Readings:** 

* Schneider, S., Lee, J. H., & Mathis, M. W. (2023). Learnable latent embeddings for joint behavioural and neural analysis. Nature, 617(7960), 360-368.

**Python prerequisites:**

* installing and importing `libraries`
* plotting with `matplotlib` library

**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/7_handson_navigation_manifold_discovery_driven_analysis_rat.ipynb).



## **8. Hands-on: navigation neural manifold with hypothesis testing in rat's HPC**

**Learning outcomes:**
  * know how to perform a more targetted <u>hypothesis-driven analyses</u>, with `CEBRA-Behavior` mode. We will qualitatively test whether both position and direction are encoded in the rat Hippocampus, by using a <u>control</u> manifold.
  
**Readings:** 

* Schneider, S., Lee, J. H., & Mathis, M. W. (2023). Learnable latent embeddings for joint behavioural and neural analysis. Nature, 617(7960), 360-368. see [Figure 2](https://cebra.ai/docs/cebra-figures/figures/Figure2.html) in Schneider, Lee, Mathis.

**Python prerequisites:**

* installing and importing `libraries`
* plotting with `matplotlib` library

**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/8_handson_navigation_manifold_hypothesis_testing_rat_part1.ipynb).




## **9. Hands-on: navigation manifold model selection in rat's HPC**

**Learning outcomes:**

  * Know how to <u>evaluate several hypotheses and select the best</u>. We will test whether position only, direction only and position and direction are encoded in the rat Hippocampus.

**Readings:** 

  * Schneider, S., Lee, J. H., & Mathis, M. W. (2023). Learnable latent embeddings for joint behavioural and neural analysis. Nature, 617(7960), 360-368. see [Figure 2](https://cebra.ai/docs/cebra-figures/figures/Figure2.html) in Schneider, Lee, Mathis.

**Python prerequisites:**

* installing and importing `libraries`
* plotting with `matplotlib` library

**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/9_handson_navigation_manifold_model_selection_rat.ipynb).




## **10. Hands-on: Hybrid approach**

**Learning outcomes**:  

  * know how to use <u>CEBRA-Hybrid</u>. We will test whether position and direction and time are encoded in the rat Hippocampus.

**Readings:** 

  * Schneider, S., Lee, J. H., & Mathis, M. W. (2023). Learnable latent embeddings for joint behavioural and neural analysis. Nature, 617(7960), 360-368. see [Figure 2](https://cebra.ai/docs/cebra-figures/figures/Figure2.html) in Schneider, Lee, Mathis.

**Python prerequisites:**

* installing and importing `libraries`
* plotting with `matplotlib` library

**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/10_handson_navigation_manifold_hybrid_rat.ipynb).




## **11. Hands-on: Manifold's consistency**

**Learning outcomes**:  
  
  * know how to use CEBRA to measure the <u>consistency</u> of manifolds across subjects.

**Readings:** 

  * Schneider, S., Lee, J. H., & Mathis, M. W. (2023). Learnable latent embeddings for joint behavioural and neural analysis. Nature, 617(7960), 360-368. see [Figure 1](https://cebra.ai/docs/cebra-figures/figures/Figure1.html) in Schneider, Lee, Mathis.

**Python prerequisites:**

  * installing and importing `libraries`
  * plotting with `matplotlib` library
  
**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/11_handson_navigation_manifold_consistency_metrics_rat_hpc.ipynb).





## 12. Hands-on: more data and generalizable encoding


**Learning outcomes**:  
  
  * Know when and how to <u>merge multiple sessions</u> of a subject together
  * Practice the use of `consistency metrics`
    
**Readings:** 

  * Schneider, S., Lee, J. H., & Mathis, M. W. (2023). Learnable latent embeddings for joint behavioural and neural analysis. Nature, 617(7960), 360-368. see [Figure 1](https://cebra.ai/docs/cebra-figures/figures/Figure1.html) in Schneider, Lee, Mathis.

**Python prerequisites:**

  * installing and importing `libraries`
  * using `functions`
  * plotting with `matplotlib` library
  
**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/12_handson_more_data_and_generalizable_encoding.ipynb).





## **13. Theory: Topology data analysis**

**Learning outcomes:** 

  * Know the basic <u>concepts</u> and <u>techniques</u> of <u>topological data analysis</u> (`simplexes`, `N-dimensional holes`, `Filtration`, `Persistent diagram`, `barcodes`)
  * Know how to use `teaspoon` to create synthetic ground truth manifolds.
  * Know how to use `ripser` software to run <u>topological analysis techniques</u> to compute the `Persistent diagram` and a manifold's `barcode`.
    
**Readings:** 

  * Schneider, S., Lee, J. H., & Mathis, M. W. (2023). Learnable latent embeddings for joint behavioural and neural analysis. Nature, 617(7960), 360-368. see [Figure 1](https://cebra.ai/docs/cebra-figures/figures/Figure1.html) in Schneider, Lee, Mathis.
  * Curto, C. What can topology tell us about the neural code? Bull. Am. Math. Soc 54, 63–78 (2016).
  * Rybakkena, E., Baasa, N., & Dunnb, B. (2017). Decoding of neural data using cohomological learning.
  * Gardner, R. J., Hermansen, E., Pachitariu, M., Burak, Y., Baas, N. A., Dunn, B. A., ... & Moser, E. I. (2022). Toroidal topology of population activity in grid cells. Nature, 602(7895), 123-128.
  * Damrich, S., Berens, P., & Kobak, D. (2023). Persistent homology for high-dimensional data based on spectral methods. arXiv preprint arXiv:2311.03087.
  ISO 690

**Python prerequisites**:

  * installing and importing `libraries`
  * plotting with `matplotlib` library

**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/13_Theory_topological_data_analysis.ipynb).


    
## **14. Hands-on: Topology data analysis**

**Learning outcomes**:

  * know how to <u>describe the topological structure of neural manifolds</u> by using `persistent homology analysis` (N-dimensional holes or co-cycles, barcodes, Betti numbers).
  * know how to visualize CEBRA embeddings into circular coordinates.

**Readings**:

  * Schneider, S., Lee, J. H., & Mathis, M. W. (2023). Learnable latent embeddings for joint behavioural and neural analysis. Nature, 617(7960), 360-368. see [Figure 2.e.-g.](https://cebra.ai/docs/cebra-figures/figures/Figure2.html) of Schneider, Lee, Mathis.
  * Curto, C. What can topology tell us about the neural code? Bull. Am. Math. Soc 54, 63-78 (2016).
  * Rybakkena, E., Baasa, N., & Dunnb, B. (2017). Decoding of neural data using cohomological learning.
  * Gardner, R. J., Hermansen, E., Pachitariu, M., Burak, Y., Baas, N. A., Dunn, B. A., ... & Moser, E. I. (2022). Toroidal topology of population activity in grid cells. Nature, 602(7895), 123-128.

**Python prerequisites**:

  * installing and importing `libraries`
  * plotting with `matplotlib` library

**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/14_handson_topology_data_analysis.ipynb).



## **15. Hands-on: Model selection with decoding accuracy**

**Learning outcomes**:

  * know how to <u>decode labels</u> from a CEBRA manifold with the `kNN`
  technique.
  * know how to ensure <u>robust decoding</u> with `cross-validation`.
  * know how to <u>evaluate and compare the decoding performances</u> for neural manifolds obtained from different hypotheses with `decoding median error` and `InfoNCE loss`.

**Readings**: 

  * Schneider, S., Lee, J. H., & Mathis, M. W. (2023). Learnable latent embeddings for joint behavioural and neural analysis. Nature, 617(7960), 360-368. see [Figure 2.d.](https://cebra.ai/docs/cebra-figures/figures/Figure2.html) of Schneider, Lee, Mathis.

**Python prerequisites**:

  * installing and importing `libraries`
  * plotting with `matplotlib` library

**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/15_handson_model_selection_with_decoding.ipynb).



## **16. Hands-on: Decoding movies from V1**

**Learning outcomes**:

  * Extract neural manifolds for different neural recording modalities (ca-imaging and neuropixels)
  * Compare neural manifolds in V1 evoked by movies features (DINO features) for different recording modalities
  * Extract neural manifolds that are consistent across neural recording modalities (Joint training)
  * Decode movie frames
  * Measure the inter and intra-area `linear consistencies` of the neural manifolds

**Readings**:

  * de Vries, S. E., Lecoq, J. A., Buice, M. A., Groblewski, P. A., Ocker, G. K., Oliver, M., ... & Koch, C. (2020). A large-scale standardized physiological survey reveals functional organization of the mouse visual cortex. Nature neuroscience, 23(1), 138-151.
  * Schneider, S., Lee, J. H., & Mathis, M. W. (2023). Learnable latent embeddings for joint behavioural and neural analysis. Nature, 617(7960), 360-368.

**Python prerequisites**:

  * installing and importing `libraries`
  * using `functions`
  * plotting with `matplotlib` library
  * machine learning with `scikit-learn` and `pytorch` libraries

**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/16_handson_decoding_V1.ipynb).



## **17. Hands-on: Information capacity**

**Learning outcomes**:

  * Extract neural manifolds for different neural recording modalities (ca-imaging and neuropixels)
  * Compare neural manifolds in V1 evoked by movies features (DINO features) for different recording modalities
  * Extract neural manifolds that are consistent across neural recording modalities (Joint training)
  * Decode movie frames
  * Measure the inter and intra-area `linear consistencies` of the neural manifolds





**Learning outcomes**

  * Know how to train a deep learning model for object recognition
  * Know how to measure its layers' neural manifold geometry (`dimensionality`, `radius`, `correlation`)
  * Know how to measure its `information capacity`

* **Readings**

  * Stephenson, C., Feather, J., Padhy, S., Elibol, O., Tang, H., McDermott, J., & Chung, S. (2019). Untangling in invariant speech recognition. Advances in neural information processing systems, 32.
  * https://github.com/steevelaquitaine/neural_manifolds_replicaMFT_Cajal/blob/master/examples/MFTMA_VGG16_example.ipynb

**Python prerequisites**:

  * installing and importing `libraries`
  * using `functions`
  * plotting with `matplotlib` library
  * machine learning with `scikit-learn` and `pytorch` libraries

**Notebook**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/steevelaquitaine/cajal_teaching/blob/main/17_handson_information_capacity.ipynb).



## Hands-on: Use Allen Institute SDK

## Hands-on: Use Dandi Archive

## Hands-on: Use Figshare

## Hands-on: Use dataryad
