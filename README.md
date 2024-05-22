# D3code
This repository contains data resources for the following paper: 

- [GeniL: A Multilingual Dataset on Generalizing Language](https://arxiv.org/pdf/2404.05866) (under review).

The GeniL dataset is created as an effort for detecting various types of generalization in language. 
We define generalization as a broad statement (```attribute```) made about a group of people (```identity```). 
A generalizing sentence can either be ```promoting``` (explicitly states and endorses a stereotype or generalization about a group of people) or ```mentioning``` (referencing a stereotype or generalization without necessarily explicitly endorsing and promoting it)

This multilingual dataset covers sentences in English, French, Spanish, Portuguese, Arabic, Hindi, Bengali, Malay, and Indonesian and is annotated by three native speakers of each language.
Each sentence is collected from a public corpora of language (mC4; multilingual Common Crawl) and contains at least one identity group name and an attribute.

# Dataset Description

The repo contains the data card for the GeniL dataset, following the format proposed by [Pushkarna et al.](https://arxiv.org/abs/2204.01075). The data card includes details of the dataset such as intended usage, field names and meanings, annotator recruitment and payments. 
Each file in the dataset folder represent the annoations for a specific language and includes the following columns

- ```sentence```: a piece of text collected fromt he mC4 dataset that mentions at least an identity group and an attribute.
- ```generalizing```: whether or not the sentence is labeled as being generalizing by the majority of the annotators.
- ```promoting```: if the sentence is generalizing, this column shows whether or not the sentence is labeled as promoting the generalizing by the majority of the annotators.
- ```identity```: if the sentence is generalizing, this column shows the identity group that the generalization is about.
- ```attribute```: if the sentenc is generalizing, this columns shows the generalization that is being made about the identity group.

  
# Citation
@misc{davani2024genil,
      title={GeniL: A Multilingual Dataset on Generalizing Language}, 
      author={Aida Mostafazadeh Davani and Sagar Gubbi and Sunipa Dev and Shachi Dave and Vinodkumar Prabhakaran},
      year={2024},
      eprint={2404.05866},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
