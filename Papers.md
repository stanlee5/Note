### A Neural Transducer (NIPS 2016) ###
- 날짜 : 2016.12

- 개요: 보다 일반적인 형태의 rnn language 모델 제안

- 동기: 기존의 seq2seq learning은 모든 입력을 받은 이후 output을 생성하는 구조로, 긴 길이를 갖는 input/output 이나 추가로 입력이 들어오는 상황(ex. 실시간 변역) 에는 적합하지 않았음

- 방법: 일정 블록 크기의 input들에 대해, attention을 적용하여 1~k개의 token을 생성함(end token을 포함하므로, 실질적인 token이 생성되지 않을 수도 있음). 2차원 형태의 Dynamic programming을 사용하여, 각 블록에서 얼마나 token을 생성할지를 결정함

- 생각: 1.Dynamic programming을 이용한 부분에서 매우 오랜 시간이 걸려서, TPU 등이 꼭 필요할 것 같음. 2.매우 흥미로운 논문임

### Auto-encoding variational bayes (ICLR 2014) ###
-
### Coherent Dialogue with Attention-based Language Models (AAAI 2017)
- 개요 : RNN에 attention을 더한 language modeling

- 동기 : 

- 방법 : 

- 생각 : 1.단순 attention도 매우 좋은 것이 신기함.

### Continuous Control with Deep Reinforcement Learning (ICLR2016)


### Convolutional Neural Network Architectures for Matching Natural Language Sentences (NIPS 2014)

### Convolutional Neural Networks for Sentence Classification (EMNLP2014) ###
- 날짜 : 2016.06

- 개요 : CNN을 활용한 sentence classification

- 동기 : 좋은 performance를 내는 CNN을 text에 적용해도 잘 될 것임

- 방법 : 단일 sentence에 cnn을 적용함. sentence를 word vector의 시퀀스로 보고, pre-train 된 word vector 위에 cnn을 적용하는데, cnn 학습이 진행되면서 word vector도 바뀔 수 있음

- 생각 : 1.cnn이 filter를 학습하면서 구조적 분석을 잘 하는 듯.



### Distributed Representations of Sentences and Documents (ICML2014) ###
- 날짜 : 2016.02

- 개요 : Word2vec 모델을 확장하여, text를 모델링하기 위한 방법

- 동기 : 텍스트 내부의 context가 주어졌을 때, context에 이어지는 단어를 예측하도록 하여 그 텍스트를 나타낼 수 있다.

- 방법 : 텍스트 내에 context(sliding window)를 뽑고, paragraph vector와 context 내 단어들을 concatenate/average 시킨 결과가 context에 이어지는 단어를 예측할 수 있도록 vector 학습

- 생각 : 1.paragraph vector를 얻기 위해서는 단순 forward 시키는 것이 아니라 network를 학습해야 하는데, 시간이 얼마나 걸릴까? 2.document를 나타내는 vector 그 자체를 얻기에는 유용해 보임



