# Awesome-Sentence-Embedding
A curated list of research papers in Sentence Reprsentation Learning.
The leaderboard of Unsupervised STS is also available.

## Content
* [Unsupervised STS benchmark](https://github.com/Doragd/Awesome-Sentence-Embedding#Unsupervised-STS-benchmark)
  * [BERT-base](https://github.com/Doragd/Awesome-Sentence-Embedding#BERT-base)
  * [BERT-large](https://github.com/Doragd/Awesome-Sentence-Embedding#BERT-large)
  * [RoBERTa-base](https://github.com/Doragd/Awesome-Sentence-Embedding#RoBERTa-base)
  * [RoBERTa-large](https://github.com/Doragd/Awesome-Sentence-Embedding#RoBERTa-large)
* [Related Papers](https://github.com/Doragd/Awesome-Sentence-Embedding#Related-Papers)
  * [Main Track of Sentence Embeddings](https://github.com/Doragd/Awesome-Sentence-Embedding#Main-Track-of-Sentence-Embeddings)
  * [Others Track of Sentence Embeddings](https://github.com/Doragd/Awesome-Sentence-Embedding#Others-Track-of-Sentence-Embeddings)
  * [Cross-lingual Sentence Embeddings](https://github.com/Doragd/Awesome-Sentence-Embedding#Cross-lingual-Sentence-Embeddings)
  * [Cross-lingual Dense Retrieval](https://github.com/Doragd/Awesome-Sentence-Embedding#Cross-lingual-Dense-Retrieval)
  * [Misc](https://github.com/Doragd/Awesome-Sentence-Embedding#Misc)

## Unsupervised STS leaderboard
### BERT-base
|Methods|STS12|STS13|STS14|STS15|STS16|STS-B|SICK-R|avg.|
|:----|:----|:----|:----|:----|:----|:----|:----|:----|
|GloVe(avg.)|55.14|70.66|59.73|68.25|63.66|58.02|53.76|61.32|
|USE|64.49|67.8|64.61|76.83|73.18|74.92|76.69|71.22|
|CLS|21.54|32.11|21.28|37.89|44.24|20.3|42.42|31.4|
|Mean|30.87|59.89|47.73|60.29|63.73|47.29|58.22|52.57|
|first-last avg.|39.7|59.38|49.67|66.03|66.19|53.87|62.06|56.7|
|Contrastive(BT)|54.26|64.03|54.28|68.19|67.5|63.27|66.91|62.63|
|BERT-Flow|58.4|67.1|60.85|75.16|71.22|68.66|64.47|66.55|
|BERT-Whitening|57.83|66.9|60.9|75.08|71.31|68.24|63.73|66.28|
|IS-BERT|56.77|69.24|61.21|75.23|70.16|69.21|64.25|66.58|
|BSL|67.83|71.4|66.88|79.97|73.97|73.74|70.4|72.03|
|CT-BERT|61.63|76.8|68.47|77.5|76.48|74.31|69.19|72.05|
|ConSERT|64.64|78.49|69.07|79.72|75.95|73.97|67.31|72.74|
|SCD|66.94|78.03|69.89|78.73|76.23|76.3|73.18|74.19|
|SG-OPT|66.84|80.13|71.23|81.56|77.17|77.23|68.16|74.62|
|Mirror-BERT|69.1|81.1|73|81.9|75.7|78|69.1|75.4|
|SimCSE|68.4|82.41|74.38|80.91|78.56|76.85|72.23|76.25|
|MCSE+coco|71.2±1.3|79.7±0.9|73.8±0.9|83.0±0.4|77.8±0.9|78.5±0.4|72.1±1.4|76.6±0.5|
|EASE|72.8|81.8|73.7|82.3|79.5|78.9|69.7|77|
|L2P-CSR|70.21|83.25|75.42|82.34|78.75|77.8|72.65|77.2|
|DCLR|70.81|83.73|75.11|82.56|78.44|78.31|71.59|77.22|
|MoCoSE|71.58|81.4|74.47|83.45|78.99|78.68|72.44|77.27|
|InforMin-CL|70.22|83.48|75.51|81.72|79.88|79.27|71.03|77.3|
|MCSE+flickr|71.4±0.9|81.8±1.3|74.8±0.9|83.6±0.9|77.5±0.8|79.5±0.5|72.6±1.4|77.3±0.5|
|VisualCSE|71.16|83.29|75.13|81.59|80.05|80.03|71.23|77.5|
|SimCSE+GS-InfoNCE|70.12|82.57|75.21|82.89|80.23|79.7|72.7|77.63|
|MixCSE|71.71±4.04|83.14±0.72|75.49±1.25|83.64±2.32|79.00±0.16|78.48±0.82|72.19±0.46|77.66±0.61|
|PT-BERT|71.2|83.76|76.34|82.63|78.9|79.42|71.94|77.74|
|AudioCSE|71.65|84.27|76.69|83.22|78.69|79.94|70.49|77.85|
|ArcCSE|72.08|84.27|76.25|82.32|79.54|79.92|72.39|78.11|
|miCSE|71.71|83.09|75.46|83.13|80.22|79.7|73.62|78.13|
|PCL|72.74|83.36|76.05|83.07|79.26|79.72|72.75|78.14|
|ESimCSE|73.4|83.27|77.25|82.66|78.81|80.17|72.3|78.27|
|DiffCSE|72.28|84.43|76.47|83.9|80.54|80.59|71.23|78.49|
|PromptBERT|71.56|84.58|76.98|84.47|80.6|81.6|69.87|78.54|
|SNCSE|70.67|84.79|76.99|83.69|80.51|81.35|74.77|78.97|
|Prompt+L2P-CSR|72.34|84.81|78.13|84.16|80.58|82.04|71.13|79.03|
|RankCSE_listNet|74.38|85.97|77.51|84.46|81.31|81.46|75.26|80.05|
|RankEncoder|74.88|85.59|78.61|83.5|80.56|81.55|75.78|80.07|
|RankCSE_listMLE|75.66|86.27|77.81|84.74|81.1|81.8|75.13|80.36|

### BERT-large
|Methods|STS12|STS13|STS14|STS15|STS16|STS-B|SICK-R|avg.|
|:----|:----|:----|:----|:----|:----|:----|:----|:----|
|CLS|27.44|30.76|22.59|29.98|42.74|26.75|43.44|31.96|
|Mean|27.67|55.79|44.49|51.67|61.88|47|53.85|48.9|
|Contrastive(BT)|52.04|62.59|54.25|71.07|66.71|63.84|66.53|62.43|
|BERT-Flow|62.82|71.24|65.39|78.98|73.23|72.72|63.77|70.07|
|BERT-Whitening|64.34|74.6|69.64|74.68|75.9|72.48|60.8|70.35|
|SG-OPT|67.02|79.42|70.38|81.72|76.35|76.16|70.2|74.46|
|ConSERT|70.69|82.96|74.13|82.78|76.66|77.53|70.37|76.45|
|SimCSE|70.88|84.16|76.43|84.5|79.76|79.26|73.88|78.41|
|MixCSE|72.55±0.49|84.32±0.53|76.69±0.76|84.31±0.10|79.67±0.28|79.90±0.18|74.07±0.13|78.80±0.09|
|DCLR|71.87|84.83|77.37|84.7|79.81|79.55|74.19|78.9|
|L2P-CSR|71.44|85.09|76.88|84.71|80|79.75|74.55|78.92|
|SimCSE+GS-InfoNCE|73.75|85.09|77.35|84.44|79.88|79.94|73.48|78.96|
|MoCoSE|74.5|84.54|77.32|84.11|79.67|80.53|73.26|79.13|
|ESimCSE|73.21|85.37|77.73|84.3|78.92|80.73|74.89|79.31|
|ArcCSE|73.17|86.19|77.9|84.97|79.43|80.45|73.5|79.37|
|PromptBERT|73.29|86.39|77.9|85.18|79.97|81.92|71.26|79.42|
|Prompt+L2P-CSR|73.14|86.78|78.67|85.77|80.32|82.23|72.57|79.93|
|PCL|74.89|85.88|78.33|85.3|80.13|81.39|73.66|79.94|
|SNCSE|71.94|86.66|78.84|85.74|80.72|82.29|75.11|80.19|
|RankCSE_listNet|74.75|86.46|78.52|85.41|80.62|81.4|76.12|80.47|
|RankCSE_listMLE|75.48|86.5|78.6|85.45|81.09|81.58|75.53|80.6|
### RoBERTa-base
|Methods|STS12|STS13|STS14|STS15|STS16|STS-B|SICK-R|avg.|
|:----|:----|:----|:----|:----|:----|:----|:----|:----|
|CLS|16.67|45.57|30.36|55.08|56.98|45.41|61.89|44.57|
|Mean|32.11|56.33|45.22|61.34|61.98|54.53|62.03|53.36|
|BERT-Whitening|46.99|63.24|57.23|71.36|68.99|61.36|62.91|61.73|
|DeCLUTR|52.41|75.19|65.52|77.12|78.63|72.41|68.62|69.99|
|BSL|68.47|72.41|68.48|78.5|72.77|78.77|69.97|72.76|
|SG-OPT|62.57|78.96|69.24|79.99|77.17|77.6|68.42|73.42|
|SCD|63.53|77.79|69.79|80.21|77.29|76.55|72.1|73.89|
|Contrastive(BT)|62.34|78.6|68.65|79.31|77.49|79.93|71.97|74.04|
|Mirror-BERT|66.6|82.7|74|82.4|79.7|79.6|69.7|76.4|
|SimCSE|70.16|81.77|73.24|81.36|80.65|80.22|68.56|76.57|
|EASE|70.9|81.5|73.5|82.6|80.5|80|68.4|76.8|
|VaSCL|69.02|82.38|73.93|82.54|80.96|69.4|80.52|76.96|
|InforMin-CL|69.79|82.57|73.36|80.91|81.28|81.07|70.3|77.04|
|ESimCSE|69.9|82.5|74.68|83.19|80.3|80.99|70.54|77.44|
|MCSE+coco|70.2±1.7|82.0±0.7|75.5±1.2|83.0±0.6|81.5±0.7|80.8±1.0|69.9±0.6|77.6±0.8|
|SimCSE+GS-InfoNCE|71.12|83.24|75|82.61|81.36|81.26|69.62|77.74|
|L2P-CSR|71.69|82.43|74.55|82.15|81.81|81.36|70.22|77.74|
|AudioCSE|68.44|83.96|75.77|82.38|82.07|81.63|70.56|77.83|
|DCLR|70.01|83.08|75.09|83.66|81.06|81.86|70.33|77.87|
|VisualCSE|70.41|83.51|74.87|82.79|81.67|81.89|69.95|77.87|
|PCL|71.54|82.7|75.38|83.31|81.64|81.61|69.19|77.91|
|DiffCSE|70.05|83.43|75.49|82.81|82.12|82.38|71.19|78.21|
|MCSE+flickr|71.7±0.2|82.7±0.4|75.9±0.3|84.0±0.4|81.3±0.3|82.3±0.5|70.3±1.3|78.3±0.1|
|CARDS|72.49|84.09|76.19|82.98|82.11|82.25|70.65|78.68|
|PromptBERT|73.94|84.74|77.28|84.99|81.74|81.88|69.5|79.15|
|SNCSE|70.62|84.42|77.24|84.85|81.49|83.07|72.92|79.23|
|RankCSE_listMLE|72.74|84.24|75.99|84.68|82.88|83.16|71.77|79.35|
|RankCSE_listNet|72.88|84.5|76.46|84.67|83|83.24|71.67|79.49|
|Prompt+L2P-CSR|74.97|83.63|78.28|84.86|82.03|82.77|71.26|79.69|
### RoBERTa-large
|Methods|STS12|STS13|STS14|STS15|STS16|STS-B|SICK-R|avg.|
|:----|:----|:----|:----|:----|:----|:----|:----|:----|
|CLS|19.25|22.97|14.93|33.41|38.01|12.52|40.63|25.96|
|Mean|33.63|57.22|45.67|63|61.18|47.07|58.38|52.31|
|Contrastive(BT)|57.6|72.14|62.25|71.49|71.75|77.05|67.83|68.59|
|BERT-Whitening|64.17|73.92|71.06|76.4|74.87|71.68|58.49|70.08|
|SG-OPT|64.29|76.36|68.48|80.1|76.6|78.14|67.97|73.13|
|InforMin-CL|70.91|84.2|75.57|82.26|79.68|81.1|72.81|78.08|
|SimCSE|72.86|83.99|75.62|84.77|81.8|81.98|71.26|78.9|
|VaSCL|73.36|83.55|77.16|83.25|80.66|72.96|82.36|79.04|
|SimCSE+GS-InfoNCE|71.76|84.91|76.79|84.35|81.74|82.97|71.71|79.21|
|DCLR|73.09|84.57|76.13|85.15|81.99|82.35|71.8|79.3|
|PCL|73.76|84.59|76.81|85.37|81.66|82.89|70.33|79.34|
|PromptBERT|73.24|83.08|77.97|84.03|81.57|82.85|73.28|79.43|
|ESimCSE|73.2|84.93|76.88|84.86|81.21|82.79|72.27|79.45|
|AudioCSE|72.1|84.3|76.74|85.11|82.51|82.94|72.45|79.45|
|L2P-CSR|73.29|84.08|76.65|85.47|82.7|82.15|72.36|79.53|
|VisualCSE|73.09|84.77|77.09|85.47|82.06|83.26|72.23|79.71|
|Prompt+L2P-CSR|73.65|84.08|78.29|85.36|82.15|83.7|73.47|80.1|
|RankCSE_listMLE|73.4|85.34|77.25|85.45|82.64|84.14|72.92|80.16|
|RankCSE_listNet|73.23|85.08|77.5|85.67|82.99|84.2|72.98|80.24|
|CARDS|74.63|86.27|79.25|85.93|83.17|83.86|72.77|80.84|
|SNCSE|73.71|86.73|80.35|86.8|83.06|84.31|77.43|81.77|

## Related Papers
### Main Track of Sentence Embeddings
```
Tips:
- 【Conf】Titile【Alias of the paper, etc.】
```
- 【ICLR2023】 RankCSE: Unsupervised Sentence Representations Learning via Learning to Rank 【RankCSE】
- 【ICLR2023】 Ranking-Enhanced Unsupervised Sentence Representation Learning 【RankEncoder】
- 【ICLR2023】 Learning to Perturb for Contrastive Learning of Unsupervised Sentence Representations 【L2P-CSR】
- 【ICLR2023】 miCSE: Mutual Information Contrastive Learning for Low-shot Sentence Embeddings 【miCSE】
- 【EMNLP2022】 Improved Universal Sentence Embeddings with Prompt-based Contrastive Learning and Energy-based Learning 【PromCSE, Supervised STS】
- 【COLING2022】 Smoothed contrastive learning for unsupervised sentence embedding 【GS-InfoNCE】
- 【COLING2022】 ESimCSE: Enhanced Sample Building Method for Contrastive Learning of Unsupervised Sentence Embedding 【ESimCSE】
- 【COLING2022】 An information minimization contrastive learning model for unsupervised sentence embeddings learning 【InforMin-CL】
- 【NIPS2022】 Non-Linguistic Supervision for Contrastive Learning of Sentence Embeddings 【VisualCSE, AudioCSE, more data】
- 【SIGIR2022】 Improving Contrastive Learning of Sentence Embeddings with Case-Augmented Positives and Retrieved Negatives 【CARDS】
- 【AAAI2022】 Unsupervised Sentence Representation via Contrastive Learning with Mixing Negatives 【MixCSE】
- 【ACL2022】 A contrastive framework for learning sentence representations from pairwise and triple-wise perspective in angular space 【ArcCSE】
- 【ACL2022】 Debiased contrastive learning of unsupervised sentence representations 【DCLR】
- 【ACL2022】 Virtual augmentation supported contrastive learning of sentence representations 【VaSCL】
- 【ACL2022】 Scd: Self-contrastive decorrelation for sentence embeddings 【SCD】
- 【ACL2022】 Exploring the impact of negative samples of contrastive learning: A case study of sentence embedding 【MoCoSE】
- 【ACL2022】 A Sentence is Worth 128 Pseudo Tokens: A Semantic-Aware Contrastive Learning Framework for Sentence Embeddings 【PT-BERT】
- 【ACL2022】 Sentence-T5: Scalable Sentence Encoders from Pre-trained Text-to-Text Models 【ST5, Supervised STS】
- 【NAACL2022】 DiffCSE：Difference-based Contrastive Learning for Sentence Embeddings 【DiffCSE】
- 【NAACL2022】 EASE: Entity-Aware Contrastive Learning of Sentence Embedding 【EASE】
- 【NAACL2022】 MCSE: Multimodal Contrastive Learning of Sentence Embeddings 【MCSE, more data】
- 【ICML2022ws】 Boosting Monolingual Sentence Representation with Large-scale Parallel Translation Datasets 【BMSR, Supervised STS, more data】
- 【Arxiv2022】 PromptBERT: Improving BERT Sentence Embeddings with Prompts 【PromptBERT】
- 【Arxiv2022】 SNCSE: Contrastive Learning for Unsupervised Sentence Embedding with Soft Negative Samples 【SNCSE】
- 【Arxiv2022】 PCL: Peer-Contrastive Learning with Diverse Augmentations for Unsupervised Sentence Embeddings 【PCL】
- 【ICLR2021】 Trans-encoder: Unsupervised sentence-pair modelling through self-and mutual-distillations 【TENC, use unlabeled STS data】
- 【ICLR2021】 Semantic re-tuning with contrastive tension 【CT-BERT】
- 【Arxiv2021】 Whitening sentence representations for better semantics and faster retrieval 【BERT-whitening】
- 【Arxiv2021】 DisCo: Effective Knowledge Distillation For Contrastive Learning of Sentence Embeddings 【DisCo, Supervised STS】
- 【EMNLP2021】 Locality Preserving Sentence Encoding 【SBERT-LP, Supervised STS】
- 【EMNLP2021】 Universal Sentence Representation Learning with Conditional Masked Language Model 【CMLM, Supervised STS】
- 【EMNLP2021】 PAUSE: Positive and Annealed Unlabeled Sentence Embedding 【PAUSE, Supervised STS】
- 【EMNLP2021】 SimCSE: Simple contrastive learning of sentence embeddings 【SimCSE】
- 【EMNLP2021】 Fast, effective, and self-supervised: Transforming masked language models into universal lexical and sentence encoders 【Mirror-BERT】
- 【EMNLP2021】 Pairwise Supervised Contrastive Learning of Sentence Representations 【PairSupCon, Supervised STS】
- 【NAACL2021】 Disentangling Semantics and Syntax in Sentence Embeddings with Pre-trained Language Models 【ParaBART, Supervised STS】
- 【ACL2021】 ConSERT: A contrastive framework for self-supervised sentence representation transfer 【ConSERT, use unlabeled STS data】
- 【ACL2021】 DeCLUTR: Deep contrastive learning for unsupervised textual representations 【DeCLUTR】
- 【ACL2021】 Bootstrapped unsupervised sentence representation learning 【BSL, Unsup & Sup】
- 【ACL2021】 Self-guided contrastive learning for bert sentence representations 【SG-OPT】
- 【SIGIR2021】 Dual-View Distilled BERT for Sentence Embedding 【DvBERT, Supervised STS】
- 【EMNLP2020】 On the sentence embeddings from pre-trained language models 【BERT-flow】
- 【EMNLP2020】 An unsupervised sentence embedding method by mutual information maximization 【IS-BERT】
- 【TASLP2020】 SBERT-WK: A Sentence Embedding Method by Dissecting BERT-Based Word Models 【SBERT-WK, Supervised STS】
- 【EMNLP2019】 Sentence-bert: Sentence embeddings using siamese bert-networks 【SBERT】
- 【ICLR2018】 An efficient framework for learning sentence representations 【Quick-thought】
- 【EMNLP2018】 Universal Sentence Encoder for English 【USE】
- 【EMNLP2017】 Supervised learning of universal sentence representations from natural language inference data 【InferSent】
- 【ACL2016】 Learning distributed representations of sentences from unlabelled data 【FastSent】
- 【NIPS2015】 Skip-thought vectors 【Skip-thought】

### Others Track of Sentence Embeddings

- 【ACL2022】 Compressing Sentence Representation for Semantic Retrieval via Homomorphic Projective Distillation
- 【NAACL2022】 Learning Dialogue Representations from Consecutive Utterances
- 【NAACL2022】 On the Effectiveness of Sentence Encoding for Intent Detection Meta-Learning
- 【ICASSP2022】 Integrating Dependency Tree into Self-Attention for Sentence Representation
- 【ICASSP2022】 Pair-Level Supervised Contrastive Learning for Natural Language Inference
- 【Arxiv2022】 Masked Autoencoders As The Unified Learners For Pre-Trained Sentence Representation
- 【Arxiv2022】 RetroMAE: Pre-training Retrieval-oriented Transformers via Masked Auto-Encoder
- 【EMNLP2021】 A Deep Decomposable Model for Disentangling Syntax and Semantics in Sentence Representation
- 【EMNLP2021】 DialogueCSE: Dialogue-based Contrastive Learning of Sentence Embeddings
- 【EMNLP2021】 WhiteningBERT: An Easy Unsupervised Sentence Embedding Approach
- 【EMNLP2021】 TSDAE: Using Transformer-based Sequential Denoising Auto-Encoderfor Unsupervised Sentence Embedding Learning
- 【EMNLP2021】 Exploiting Twitter as Source of Large Corpora of Weakly Similar Pairs for Semantic Sentence Embeddings
- 【ACL2021】 DefSent: Sentence Embeddings using Definition Sentences
- 【ACL2021】 Discrete Cosine Transform as Universal Sentence Encoder
- 【Arxiv2021】 S-SimCSE: sampled sub-networks for contrastive learning of sentence embedding
- 【NAACL2021】 Augmented SBERT: Data augmentation method for improving bi-encoders for pairwise sentence scoring tasks
- 【Arxiv2020】 CERT: contrastive self-supervised learning for language understanding
- 【AAAI2020】 Scalable Attentive Sentence-Pair Modeling via Distilled Sentence Embedding
- 【EMNLP2020】 Cross-Thought for Sentence Encoder Pre-training
- 【WWW2020】 Enhanced-RCNN: An Efficient Method for Learning Sentence Similarity
- 【ACL2020】 QuASE: Question-Answer Driven Sentence Encoding
- 【EMNLP2019】 Efficient Sentence Embedding using Discrete Cosine Transform
- 【EMNLP2019】 Parameter-free Sentence Embedding via Orthogonal Basis
- 【EMNLP2019】 Incorporating Visual Semantics into Sentence Representations within a Grounded Space
- 【NAACL2019】 Continual Learning for Sentence Representations Using Conceptors
- 【NAACL2019】 A Multi-Task Approach for Disentangling Syntax and Semantics in Sentence Representations
- 【ACL2019】 Simple and Effective Paraphrastic Similarity from Parallel Translations
- 【ACL2019】 Learning Compressed Sentence Representations for On-Device Text Processing
- 【ACL2019】 Exploiting Invertible Decoders for Unsupervised Sentence Representation Learning

### Cross-lingual Sentence Embeddings

- 【ACL2022】 Language-agnostic BERT Sentence Embedding
- 【IJCAI2022】 Unsupervised Context Aware Sentence Representation Pretraining for Multi-lingual Dense Retrieval
- 【Arxiv2021】 Paraphrastic Representations at Scale
- 【ACL2021】 Lightweight Cross-Lingual Sentence Representation Learning
- 【ACL2021】 Bootstrapped Unsupervised Sentence Representation Learning
- 【ACL2021】 Self-Guided Contrastive Learning for BERT Sentence Representations
- 【EMNLP2021】 Fast, Effective and Self-Supervised: Transforming Masked Language Models into Universal Lexical and Sentence Encoders
- 【EMNLP2021】 Aligning Cross-lingual Sentence Representations with Dual Momentum Contrast
- 【EMNLP2021】 Cross-lingual Sentence Embedding using Multi-Task Learning
- 【EMNLP2021】 Semantic Alignment with Calibrated Similarity for Multilingual Sentence Embedding
- 【EMNLP2021】 Language-agnostic Representation from Multilingual Sentence Encoders for Cross-lingual Similarity Estimation
- 【Arxiv2021】 Analyzing Zero-shot Cross-lingual Transfer in Supervised NLP Tasks
- 【ACL2020】 Unsupervised Multilingual Sentence Embeddings for Parallel Corpus Mining
- 【AAAI2020】 Emu: Enhancing Multilingual Sentence Embeddings with Semantic Specialization
- 【AAAI2020】 Unsupervised Interlingual Semantic Representations from Sentence Embeddings for Zero-Shot Cross-Lingual Transfer
- 【AAAI2020】 ABSent: Cross-Lingual Sentence Representation Mapping with Bidirectional GANs
- 【EMNLP2020】 Making Monolingual Sentence Embeddings Multilingual using Knowledge Distillation
- 【EMNLP2020】 A Bilingual Generative Transformer for Semantic Sentence Embedding
- 【EMNLP2019】 Margin-based Parallel Corpus Mining with Multilingual Sentence Embeddings
- 【EMNLP2019】 Exploring Multilingual Syntactic Sentence Representations
- 【IJCAI2019】 Improving Multilingual Sentence Embedding using Bi-directional Dual Encoder with Additive Margin Softmax

### Cross-lingual Dense Retrieval

- 【ICLR2023】 Modeling Sequential Sentence Relation to Improve Cross-lingual Dense Retrieval
- 【ICLR2023】 LEXA: Language-agnostic Cross-consistency Training for Question Answering Tasks
- 【IJCAI2022】 Unsupervised Context Aware Sentence Representation Pretraining for Multi-lingual Dense Retrieval
- 【NAACL2022】 EASE: Entity-Aware Contrastive Learning of Sentence Embedding
- 【EMNLP2021】 A Simple and Effective Method To Eliminate the Self Language Bias in Multilingual Representations
- 【EMNLP2020】 Language-Agnostic Answer Retrieval from a Multilingual Pool

### Misc

- 【ICLR2023】 Understanding The Role of Positional Encodings in Sentence Representations
- 【ICLR2023】 Self-Consistent Learning: Cooperation between Generators and Discriminators
- 【TMLR2022】 Unsupervised dense information retrieval with contrastive learning
- 【NAACL2021】 Supporting Clustering with Contrastive Learning
