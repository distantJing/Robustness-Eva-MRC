## How to Use
## Screenshots

## Table of Contents
- [MRC models](#MRC-models)
- [Adversarial Attack Methods](#Adversarial-Attack-Methods)
- [Evaluation](#evaluation)
- [Analysis](#Analysis)


![](../src/framework.png)
Robustness-Eva-MRC, is a platform that explores the robustness of both pre-train language models (PLMs) and three large-scale language models (LLMs) in the extractive machine reading comprehension (MRC) task. 
The platform consists of four main modules: MRC Models, adversarial attack methods, evaluation, analysis.


## MRC Models
The first module is the MRC Models, which directly fetches the checkpoint files for MRC models directly from the HuggingFace repository. 
This module preloads five PLMs-based MRC models fine-tuned on the MRQA datasets and utilizs three LLMs-based in a conversational format.

It lists models's parameter scale and other information.
![](./src/1-1.png )
It also provides links to the hugging face of the corresponding model.
![](./src/1-2.png )


## Adversarial Attack Methods
This part combines eight adversarial attack methods with five MRC datasets to generate new challenging adversarial testing sets, resulting in a total of 40 diverse adversarial testing sets.

It use five extractive MRC datasets (SQuAD 1.1, HotpotQA , Natural Questions, NewsQA, TriviaQA) and lists their statistical information. 
![](./src/2-3.png )

Then it describes eight adversarial attack methods.
![](./src/2-0.png )

We also show the reconstruction method and detailed examples for each adversarial attack method.
This is a example case of WordReplace.
![](./src/2-1.png )

Besides, the platform provides the interface for generating new adversarial sets.
![](./src/2-2.png )
It provides a flexible interface to reconstruct new test sets that is interfered with by one or multiple attacks.
![](./src/2-4.png )


## Evauation

list all the results
![](./src/3-1.png )
show example case
![](./src/3-2.png )
![](./src/3-3.png )

   <!-- * evaluates the performance of the MRC models on both the original and adversarially perturbed datasets, and lists all results and supports illustrating each sample for a case study.
   * users can also download all kinds of test sets and upload their prediction files to the platform. -->


## Analysis 
   * Visualization for Single Model & Model Comparison
For pretrain language models:
![](./src/4-1.png )
![](./src/4-2.png )
![](./src/4-1-1.png )
![](./src/4-3.png )
![](./src/4-4.png )

For large-scale language models:
![](./src/4-5.png )
![](./src/4-6.png )
![](./src/4-7.png )
![](./src/4-8.png )


   * Case Studies for Single Model & Model Comparison
![](./src/5-1.png )
![](./src/5-2.png )


   * Mix Attack Analysis
![](./src/6-1.png )


