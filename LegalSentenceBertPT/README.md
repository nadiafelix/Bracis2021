# Portuguese Legislative Sentence Embedding: 
- We trained the Legal Sentence Bert for Brasilian Portuguese using a contrastive learning  framework 
- Contrastive learning is a machine learning technique used to learn the general features of a dataset without labels by teaching the model which data points are similar or different.
- We used SimCSE [1] coupled with the Portuguese pre-trained language model named  BERTimbau [2]. We use the same hyperparameters, and the training set is described next:

1) From [3], we used 215,713 comments. We removed the comments from PL 3723/2019, PEC 471/2005, and Hashtag Corpus, in order to avoid bias.
2) From [3], we also used 147,008 bills. From these projects, we used the summary field named txtEmenta and the project core text named txtExplicacaoEmenta.
3) From Political Speeches [4], we used 462,831 texts, specifically, we used the columns: sumario, textodiscurso, and indexacao.  

These corpora were segmented into sentences and concatenated, producing 2,307,426 sentences.

[1] Gao, T., Yao, X., Chen, D.: Simcse: Simple contrastive learning of sentence em-beddings (2021)

[2]  Souza,  F.,  Nogueira,  R.,  Lotufo,  R.:  BERTimbau:  pretrained  BERT  modelsfor  Brazilian  Portuguese.  In:  9th  Brazilian  Conference  on  Intelligent  Systems,BRACIS, Rio Grande do Sul, Brazil, October 20-23(2020)

[3] Câmara dos Deputados (Brazilian Chamber of Deputies, when translated to En-glish): Popular participation. https://www2.camara.leg.br/transparencia/servicos-ao-cidadao/participacao-popular (2021), accessed: 2021-05-05

## Authors 
LegalSentenceBertPT-BR was trained and evaluated by Nádia Félix F. da Silva, Marília Costa Rosendo Silva, Fabíola Pereira, João Tarrega, João Vitor Pataca Beinotti,  Marcio Rodrigo Fernandes de Moraes Fonseca, Francisco Edmundo de Andrade, and André Carlos Ponce de Leon Ferreira de Carvalho.

## Citation
If you use our work, please cite:
```bibtex
@inproceedings{LegalSentenceBertPT-BR,
  title={Evaluating Topic Models in Portuguese Political Comments about Bills from Brazil's Chamber of Deputies},
  author={Silva, Nadia F. F. da and Silva, Marília Costa Rosendo and Pereira, Fabíola and Tarrega, João Pedro and Beinotti, João Vitor Pataca and Fonseca, Marcio Rodrigo Fernandes de Moraes and Andrade, Francisco Edmundo de and Caravalho, André Carlos Ponce de Leon Ferreira},
  booktitle={10th  Brazilian  Conference  on  Intelligent  Systems, BRACIS, São Carlos- SP, Brazil},
  year={2021}
}
```


