# Exploring the BERT Cross-Lingual Transfer for Reading Comprehension

Multilingual BERT has been shown to generalize well in a zero-shot cross-lingual setting. This generalization was measured on POS and NER tasks. 
We explore the multilingual BERT cross-language transferability on the reading comprehension task. We compare different modes of training of 
question-answering model for a non-English language using both English and language-specific data. We demonstrate that the model based on 
multilingual BERT is slightly behind the monolingual BERT-based on Russian data, however, it achieves comparable results with the language-specific 
variant on Chinese. We also show that training jointly on English data and additional 10,000 monolingual samples allows it to reach the performance 
comparable to the one trained on monolingual data only.

### Using

The repository contains:

* `ch-bert-base-chinese.json` -- DeepPavlov configuration file for the Chinese language squad based on DRCD.
* `en-bert-base-cased.json` -- DeepPavlov configuration file for the English language squad.
* `ru-DeepPavlov-rubert-base-cased.json` -- DeepPavlov configuration file for the Russian language squad SberQuAD.


To execute the model install DeepPavlov by running:
`pip install deeppavlov`

To run inference execute:
`python -m deeppavlov evaluate {config_name}`


### Contact
For any question, please contact vaskoncv@gmail.com


### Cite

```yaml
@inproceedings{konovalov2020squad,
  title={Exploring the BERT Cross-Lingual Transfer for Reading Comprehension},
  author={Konovalov, Vasily and Gulyaev, Pavel and Sorokin, Alexey and Kuratov, Yury and Burtsev, Mikhail},
  booktitle={Komp'juternaja Lingvistika i Intellektual'nye Tehnologii},
  year={2020},
  pages={445--453},
  authorscopus={true},
}


