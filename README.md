# TFM — From sound to feeling: a computational psychological approach to mood prediction and classification in music

This repository contains the end-to-end workflow for my Master’s Thesis on how raw audio can be transformed into psychologically meaningful mood predictions using computational methods. The project focuses on extracting acoustic and mid-level perceptual features from Mel spectrograms, training interpretable models, and linking results back to psychological theories of emotional perception. 

*Project overview*

- Goal: Model and interpret the relationship between audio features (tempo, spectral descriptors, harmonic content) and perceived mood in music; accuracy matters, but interpretability is central. 
- Why it matters: Bridges psychology, cognitive science, and ML/affective computing. 
- What we expect: Identify which perceptual features align with moods having an interpretable base, and reveal structured acoustic patterns behind mood perception.

*Data source*

- We used MTG-Jamendo (≈55k full tracks with mood, genre, instrument tags). We start from pre-computed Mel spectrograms and metadata; later, we also use MP3 audio to derive additional features. Mood annotations serve as the ground truth for supervised learning and for psychological interpretation. 
- Data and licensing: Audio/Mel files are not included in this repo due to size and licenses. If you want to replicate please download them from the following the included guide or following the steps in the official source. 

*Repository contents*

1. DOWNLOADING DATA.pdf: A step-by-step guide to download the Mel spectrograms and audio subsets from MTG-Jamendo. Follow the instructions and adjust only the local paths on your machine.
2. Dataset_creation.ipynb: Python notebook that documents how the working dataset was built (extraction of acoustic features from Mel spectrograms and audio tracks, integration of mood/theme tags and additional metadata). 
3. EDA_final.rmd: R Markdown with the exploratory data analysis and modeling (descriptive statistics, data checks and distributions, baseline models, evaluation and interpretability analysis).

*Data source and licensing*

- Dataset: MTG-Jamendo (music and annotations under Creative Commons; see the dataset’s README/licenses). https://github.com/MTG/mtg-jamendo-dataset 
- Citation: Bogdanov, D., Won M., Tovstogan P., Porter A., & Serra X. (2019). The MTG-Jamendo Dataset for Automatic Music Tagging. Machine Learning for Music Discovery Workshop, International Conference on Machine Learning (ICML 2019). 
- Code in this repo is shared under MIT license.

Thank you for taking the time and interest to review this project; any comments or suggestions are welcome! :)
