## 소개
* 이 저장소는 'Word2Vec : Efficient estimation of word representations in vector space' 논문에 대한 리뷰와 간단한 구현이 있습니다.

## "Efficient Estimation of Word Representations in Vector Space" 논문 정보

- **제목:** Efficient Estimation of Word Representations in Vector Space
- **저자:** Tomas Mikolov, Kai Chen, Greg Corrado, Jeffrey Dean
- **발행년도:** 2013
- **논문 링크:** [PDF](https://arxiv.org/abs/1301.3781)

## Word2Vec이란?

* Word2Vec은 단어를 벡터로 표현하는 자연어 처리(Natural Language Processing, NLP) 기술 중 하나로, 단어 간 의미적 유사성을 수치적으로 나타냅니다. 이 기술은 단어들을 연속적인 공간에 투영하여 단어 간의 관계를 이해하고, 단어 벡터 간의 거리를 통해 의미적 유사성을 측정합니다. 
* 이 논문은 기존의 단어 표현 기법을 개선하고자 하는 목적에서 Word2Vec이라는 단어 임베딩 기술을 소개합니다. 두 가지 주요 모델인 Continuous Bag of Words (CBOW)와 Skip-gram을 제안하며, 효율적인 학습을 위한 Hierarchical Softmax와 Negative Sampling을 도입합니다. 이를 통해 대규모 텍스트 데이터에서 단어 간의 의미적 유사성을 학습하는 데 탁월한 성과를 보입니다.

## 핵심 아이디어

### 1. Word Embedding

* 논문에서 제안된 Word2Vec은 단어를 고차원 벡터로 표현하여 단어 간 의미적 유사성을 벡터 공간에 효과적으로 포착합니다.

### 2. CBOW 모델

* CBOW 모델은 주변 단어들의 임베딩을 이용하여 특정 단어를 예측하는 모델로, 주변 단어들의 평균 벡터를 입력으로 사용합니다.

### 3. Skip-gram 모델

* Skip-gram 모델은 특정 단어를 입력으로 받아 주변 단어들을 예측하는 모델로, 입력 단어를 이용해 주변 단어들을 하나씩 예측하는 방식으로 학습됩니다.

### 4. 효율적인 학습 기법

* Hierarchical Softmax와 Negative Sampling은 계산 효율성을 높이기 위해 도입되었습니다. 특히, Hierarchical Softmax는 전통적인 Softmax의 계산 복잡도를 개선하여 대규모 어휘에서도 효율적인 학습을 가능케 합니다.

## 논문에 관한 추가 자료

* Word2Vec을 소개한 Efficient estimation of word representations in vector space 논문에 대한 자세한 내용은 [논문요약자료](https://github.com/HY-AI2-Projects/Word2Vec/blob/main/Word2Vec_%EB%85%BC%EB%AC%B8%EB%A6%AC%EB%B7%B0.pdf)를 참고하세요.

## 참고 자료

- [Word2Vec: Skip-gram and CBOW](https://arxiv.org/abs/1301.3781)
- [Efficient Estimation of Word Representations in Vector Space](https://arxiv.org/abs/1301.3781)
