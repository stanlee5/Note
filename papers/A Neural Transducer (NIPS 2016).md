#### 날짜 ####
2016.12

#### 개요 ####
보다 일반적인 형태의 rnn language 모델 제안

#### 동기 ####
기존의 seq2seq learning은 모든 입력을 받은 이후 output을 생성하는 구조로, 긴 길이를 갖는 input/output 이나 추가로 입력이 들어오는 상황(ex. 실시간 변역) 에는 적합하지 않았음

#### 방법 ####
- 일정 블록 크기의 input들에 대해, attention을 적용하여 1~k개의 token을 생성함
- end token을 포함하므로, 실질적인 token이 생성되지 않을 수도 있음.
- 2차원 형태의 Dynamic programming을 사용하여, 각 블록에서 얼마나 token을 생성할지를 결정함

#### 생각 ####
- Dynamic programming을 이용한 부분에서 매우 오랜 시간이 걸려서, TPU 등이 꼭 필요할 것 같음
- 2.매우 흥미로운 논문임

#### [논문링크](https://arxiv.org/abs/1511.04868), [목록으로](https://github.com/stanlee5/Note/blob/master/Papers-summary.md) ####
