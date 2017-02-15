## Distributed Representations of Sentences and Documents (ICML2014) ##

#### 날짜 : 2016.02 ####

#### 개요 : Word2vec 모델을 확장하여, text를 모델링하기 위한 방법 ####

#### 동기 : 텍스트 내부의 context가 주어졌을 때, context에 이어지는 단어를 예측하도록 하여 그 텍스트를 나타낼 수 있다. ####

#### 방법 ####
- 텍스트 내에 context(sliding window)를 뽑고
- paragraph vector와 context 내 단어들을 concatenate/average 시킨 결과가 context에 이어지는 단어를 예측할 수 있도록 vector 학습

#### 생각 ####
- 1.paragraph vector를 얻기 위해서는 단순 forward 시키는 것이 아니라 network를 학습해야 하는데, 시간이 얼마나 걸릴까?
- 2.document를 나타내는 vector 그 자체를 얻기에는 유용해 보임
