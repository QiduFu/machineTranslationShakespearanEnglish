# Machine Translation of Shakespearean English

By Qidu Fu, Haotian Shen, Yixing (Leo) Zhu, Kiley Jolicoeur, Ed Cogan

Under Dr. Lu Xiao for Natural Language Processing

This markdown is based on the poster presented at the 2023 Poster Day of School of Information Studies at the Syracuse University. For more information of this project, see [the poster](Machine_Translation%20of%20Shakespearean_English_Poster.pdf). For the code implementation, please see [the Jupyter Notebook](Machine_Translation_of_Shakespearean_English.ipynb). 

# Outline
- [1 - Overview](#1)
- [2 - Data](#2)
  - [2.1 - Source](#2.1)
  - [2.2 - Preparation](#2.2)
    - [2.2.1 - Tokenization](#2.2.1)
    - [2.2.2 - Embedding](#2.2.2)
- [3 - Modeling](#3)
- [4 - Interpretation](#4)
- [5 - Conclusion](#5)
- [6 - References](#6)

<a name="1"></a>
## 1 - Overview
This project employs a multi-head attention model for translating Shakespearean text data from Early Modern English (late 16th to early 17th century) to Modern English. It focuses on changing the stylistic properties of the text while maintaining its content, achieving an accuracy of ~0.77 in the cross validation datasets. The model's applications include enhancing translation efficiency and accuracy and automating text style transformations.

<a name="2"></a>
## 2 - Data
<a name="2.1"></a>
### 2.1 - Source
The text data are derived from Jhamtani’s (2017) study, featuring parallel texts in Modern and Early Modern Shakespearean English with 21076 sentences in each of the texts.

<a name="2.2"></a>
### 2.2 - Preparation
<a name="2.2.1"></a>
#### 2.2.1 - Tokenization
Both the original and translated texts are tokenized into integer sequences for neural network processing.

<a name="2.2.2"></a>
#### 2.2.2 - Embedding
A combination of token embedding and positional coding represents words in the transformer model, aiding in semantic and position understanding within input sequences.

<a name="3"></a>
## 3 - Modeling
The study aims to transform Early Modern English text to Modern English, navigating the challenges of historical language translation with limited parallel texts. The use of a Transformer model (introduced by Vaswani et al., 2017) marks a significant advancement in sequence-to-sequence tasks like machine translation, particularly for natural language processing.

<a name="4"></a>
## 4 - Interpretation
Interpreting the Transformer model involves analyzing its focus on specific words or phrases during translation and understanding the hierarchical encoding of information. This process unravels the model's attention mechanisms and examines learned representations to decipher language transformation across time periods.

<a name="5"></a>
## 5 - Conclusion
The project demonstrates the successful construction of a Sequence-to-Sequence Transformer model for translating Early Modern English to Modern English, achieving an accuracy of ~0.77. This model facilitates a deeper understanding and accessibility of Shakespearean literature.

<a name="6"></a>
## 6 - References
1. Jhamtani, H., Gangal, V., Hovy, E., & Nyberg, E. (2017). Shakespearizing modern language using copy-enriched sequence-to-sequence
models. arXiv preprint arXiv:1707.01161.
2. Hu, Z., Lee, R. K. W., Aggarwal, C. C., & Zhang, A. (2022). Text style transfer: A review and experimental evaluation. ACM SIGKDD Explorations
Newsletter, 24(1), 14-45.
3. TensorFlow. (2023, November 16). Neural Machine Translation with a Transformer and Keras. Retrieved from
www.tensorflow.org/text/tutorials/transformer
4. Vaswani et al., (2017). The Transformer-model architecture. 31st Conference on Neural Information Processing Systems (NIPS2017),
https://arxiv.org/pdf/1706.03762.pdf. Accessed November 21, 2023.
5. Hong, Tao. "Coherent Wave Dynamics and Language Generation of a Generative Pre-trained Transformer" 8 May 2023, arXiv:2305.05061, Cornell
University, https://arxiv.org/abs/2305.05061. Accessed 10 Nov. 2023.
6. Jin, D., Jin, Z., Hu, Z., Vechtomova, O., Mihalcea, R. (2022). Deep Learning for Text Style Transfer: A Survey. Computational Linguistics 48 (1):
155–205. doi: https://doi.org/10.1162/coli_a_00426
7. Troiano, E., Velutharambath, A., Klinger, R. (2023). From theories on styles to their transfer in text: Bridging the gap with a hierarchical survey.
Natural Language Engineering, 29(4), 849-908. doi:10.1017/S1351324922000407
8. Early modern English: grammar, pronunciation, and spelling. Oxford English Dictionary.
https://www.oed.com/discover/early-modern-english-spelling-grammar-and-pronunciation/ Accessed 27 November 2023.
9. Domingo, M., Casacuberta, F. (2023). Interactive machine translation for the language modernization and spelling normalization of historical
documents. Pattern Anal Applic 26, 1601–1614 (2023). https://doi.org/10.1007/s10044-023-01164-w