# GeniL
This repository contains data resources for the following paper: 

- [GeniL: A Multilingual Dataset on Generalizing Language](https://arxiv.org/pdf/2404.05866) (under review).

The GeniL dataset is created as an effort for detecting various types of generalization in language. 
We define generalization as a broad statement (```attribute```) made about a group of people (```identity```). 
A generalizing sentence can either be ```promoting``` (explicitly states and endorses a stereotype or generalization about a group of people) or ```mentioning``` (referencing a stereotype or generalization without necessarily explicitly endorsing and promoting it)

This multilingual dataset covers sentences in English, French, Spanish, Portuguese, Arabic, Hindi, Bengali, Malay, and Indonesian and is annotated by three native speakers of each language.
Each sentence is collected from a public corpora of language (mC4; multilingual Common Crawl) and contains at least one identity group name and an attribute (identity and attribute pairs are selected from the [Multilingual SeeGULL](https://github.com/google-research-datasets/SeeGULL-Multilingual) dataset.)

# Dataset Description

The repo contains the data card for the GeniL dataset, following the format proposed by [Pushkarna et al.](https://arxiv.org/abs/2204.01075). The data card includes details of the dataset such as intended usage, field names and meanings, annotator recruitment and payments. 
Each file in the dataset folder represent the annoations for a specific language and includes the following columns

- ```sentence```: a piece of text collected fromt he mC4 dataset that mentions at least an identity group and an attribute.
- ```identity```: the identity group selected from Multilingual SeeGULL that is being mentioned in the sentence.
- ```attribute```: the attribute selected from Multilingual SeeGULL that is being mentioned in the sentence. 
- ```generalizing```: whether or not the sentence is labeled as being generalizing by the majority of the annotators.
- ```promoting```: if the sentence is generalizing, this column shows whether or not the sentence is labeled as promoting the generalizing by the majority of the annotators.


  
# Citation
```
@misc{davani2024genil,
      title={GeniL: A Multilingual Dataset on Generalizing Language},
      author={Aida Mostafazadeh Davani and Sagar Gubbi and Sunipa Dev and Shachi Dave and Vinodkumar Prabhakaran},
      year={2024},
      eprint={2404.05866},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```
