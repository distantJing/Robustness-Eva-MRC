# Adversarial Attack Methods
The platform integrates eight adversarial attack methods with five MRC datasets to generate new challenging adversarial testing sets. 

## Table of Contents
- [MRC Datasets](#MRC-Datasets)

## MRC Datasets
We randomly selected 1000 samples from each of the following extractive MRC datasets:
* SQuAD 1.1
* HotpotQA 
* Natural Questions
* NewsQA
* TriviaQA


## Adversarial Attacks
| Methods                                    | Attack Level | Attack Object | Transformation                                                                   | Search Method                             |
| ------------------------------------------ | ------------ | ------------- | -------------------------------------------------------------------------------- | ----------------------------------------- |
| SEARs       | Word         | Qusetion      |                                                                                  | Semantically equivalent adversarial rules |
| ModifyOption  | Word         | Passage       | Unrelated phrases insertion                                                      | Heuristic rule                            |
| Morpheus     | Word         | Qusetion      | Inflection word swap                                                             | Greedy search                             |
| Pwws         | Word         | Qusetion      | WordNet-based synonym replace                                                    | Greedy-WIR (saliency)                     |
| WordReplace                                | Word         | Passage       | WordNet-based synonym replace                                                    | Random search                             |
| Charswap  | Char         | Passage       | Neighboring character swap                                                       | Random search                             |
| Pruthi      | Char         | Qusetion      | Neighboring and keyboard-based character swap, character deletion and insertion. | Greedy search                             |
| Addsent      | Sentence     | Passage       | Distraction sentence insertion                                                   | Heuristic rule                            |


###### Detail Cases
Here we list all addversarial attack methods and the corresponding recontrution cases.


