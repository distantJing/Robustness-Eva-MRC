## Case Analysis
    The following shows a case of different models facing attacks on the SQuAD dataset.
### Comparison between baes-model and large-model
 --The Case on the left represents the model's forecast based on the unaltered data, whereas the case on the right demonstrates its prediction subsequent to undergoing an attack.
#### case show
* __BERT-base & BERT-large__
![alt 属性文本](./IMG/rule1/bert/Seras.jpg)
![alt 属性文本](./IMG/rule1/bert/Morpheus.jpg)
![alt 属性文本](./IMG/rule1/bert/Addsent.jpg)
![alt 属性文本](./IMG/rule1/bert/Charswap.jpg)
![alt 属性文本](./IMG/rule1/bert/ModifyOption.jpg)
![alt 属性文本](./IMG/rule1/bert/Pruthi.jpg)
![alt 属性文本](./IMG/rule1/bert/WordReplace.jpg)
![alt 属性文本](./IMG/rule1/bert/Pwws.jpg)
* __RoBERTa-base & RoBERTa-large__
![alt 属性文本](./IMG/rule1/roberta/Seras.jpg)
![alt 属性文本](./IMG/rule1/roberta/Morpheus.jpg)
![alt 属性文本](./IMG/rule1/roberta/Addsent.jpg)
![alt 属性文本](./IMG/rule1/roberta/Charswap.jpg)
![alt 属性文本](./IMG/rule1/roberta/ModifyOption.jpg)
![alt 属性文本](./IMG/rule1/roberta/Pruthi.jpg)
![alt 属性文本](./IMG/rule1/roberta/WordReplace.jpg)
![alt 属性文本](./IMG/rule1/roberta/Pwws.jpg)
* __ELECTRA-base & ELECTRA-large__
![alt 属性文本](./IMG/rule1/electra/Seras.jpg)
![alt 属性文本](./IMG/rule1/electra/Morpheus.jpg)
![alt 属性文本](./IMG/rule1/electra/Addsent.jpg)
![alt 属性文本](./IMG/rule1/electra/Charswap.jpg)
![alt 属性文本](./IMG/rule1/electra/ModifyOption.jpg)
![alt 属性文本](./IMG/rule1/electra/Pruthi.jpg)
![alt 属性文本](./IMG/rule1/electra/WordReplace.jpg)
![alt 属性文本](./IMG/rule1/electra/Pwws.jpg)
* __DeBERTaV3-base & DeBERTaV3-large__
![alt 属性文本](./IMG/rule1/debertav3/Seras.jpg)
![alt 属性文本](./IMG/rule1/debertav3/Morpheus.jpg)
![alt 属性文本](./IMG/rule1/debertav3/Addsent.jpg)
![alt 属性文本](./IMG/rule1/debertav3/Charswap.jpg)
![alt 属性文本](./IMG/rule1/debertav3/ModifyOption.jpg)
![alt 属性文本](./IMG/rule1/debertav3/Pruthi.jpg)
![alt 属性文本](./IMG/rule1/debertav3/WordReplace.jpg)
![alt 属性文本](./IMG/rule1/debertav3/Pwws.jpg)
#### case analysis
  * These cases show that both large-models and base-models predict correctly on the original text, but when faced with attacks, base-model predicts incorrectly and large-model predicts correctly. This suggests that Increasing the number of parameters can effectively improve model robustness.

### Comparison between large-scale language models
 --The Case on the left represents the model's forecast based on the unaltered data, whereas the case on the right demonstrates its prediction subsequent to undergoing Addsent attack.
* __Llama__
![alt 属性文本](./IMG/rule3/Llama.jpg)
* __Opt__
![alt 属性文本](./IMG/rule3/Opt.jpg)
* __ChatGpt__
![alt 属性文本](./IMG/rule3/ChatGpt.jpg)
#### case analysis
  * These cases show the predictions of Llama, Opt, ChatGpt after the original text and after being attacked by addsent. The red highlight is the label for the model's predicted answer. We discovered that the LLaMA and OPT answered incorrectly after being attacked by Addsent, indicating poor robustness under adversarial conditions. These models often generate extraneous information, such as repeated prompts, supplementary content, or information unrelated to the query at hand. In contrast, ChatGPT demonstrates exceptional robustness, significantly outperforming all other models, and generating minimal irrelevant information.

### Further MixAttacks on ChatGPT
 --The left side of the case shows the model's predictions against the addsent attack, and the right side shows the results against the mixattack attack. Here are all the cases in which ChatGpt's predictions were incorrect due to the MixAddsent attack.
* __Addsent+Pwws__
![alt 属性文本](./IMG/rule4/A%2BP.jpg)
* __ChatGpt+Addsent__
![alt 属性文本](./IMG/rule4/C%2BA.jpg)
![alt 属性文本](./IMG/rule4/C%2BA_2.jpg)
* __Pwws+ChatGpt+Addsent__
![alt 属性文本](./IMG/rule4/P%2BC%2BA.jpg)
![alt 属性文本](./IMG/rule4/P%2BC%2BA_2.jpg)
![alt 属性文本](./IMG/rule4/P%2BC%2BA_3.jpg)
#### case analysis
  * From these cases, we observed that ChatGPT does demonstrate vulnerabilities under complex text perturbations, albeit to a lesser degree than other models. Despite its superior robustness, it is not entirely immune to adversarial attacks.


## More Case
>The aforementioned section presents only a limited number of cases. However, a comprehensive compilation of all cases is currently being prepared and will be published in the near future.

