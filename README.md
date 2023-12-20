# 소개
* 이 저장소는 'Word2Vec : Efficient estimation of word representations in vector space' 논문에 대한 리뷰와 간단한 구현을 한 한양대학교 '인공지능2'수업 기말 과제입니다. 

## Word2Vec이란?

Word2Vec은 단어를 벡터로 표현하는 자연어 처리(Natural Language Processing, NLP) 기술 중 하나로, 단어 간 의미적 유사성을 수치적으로 나타냅니다. 이 기술은 단어들을 연속적인 공간에 투영하여 단어 간의 관계를 이해하고, 단어 벡터 간의 거리를 통해 의미적 유사성을 측정합니다.

## Word Embedding

Word2Vec은 단어 임베딩의 한 형태로, 단어를 고차원 벡터로 매핑하는 작업입니다. 임베딩된 단어 벡터는 단어의 의미와 관련된 정보를 포함하고 있으며, 유사한 의미를 가진 단어들은 벡터 공간에서 서로 가깝게 위치합니다.

## CBOW (Continuous Bag of Words) 모델

CBOW 모델은 주변 단어들의 임베딩을 이용하여 특정 단어를 예측하는 모델입니다. 주변 단어들의 평균 벡터를 입력으로 사용하고, 이를 통해 대상 단어를 예측합니다.

## Skip-gram 모델

Skip-gram 모델은 특정 단어를 입력으로 받아 주변 단어들을 예측하는 모델입니다. 입력 단어를 이용해 주변 단어들을 하나씩 예측하는 방식으로 학습됩니다.

## 학습 과정

Word2Vec 모델은 대량의 텍스트 데이터를 사용하여 단어 간의 관계를 학습합니다. 모델이 학습되면 단어 간 유사성 및 의미적 관계를 캡처하는 벡터 표현이 얻어집니다.

## 논문에 관한 자세한 자료

Word2Vec을 소개한 Efficient estimation of word representations in vector space 논문에 대한 자세한 내용은 [논문요약자료](https://github.com/HY-AI2-Projects/Word2Vec/blob/main/Word2Vec_%EB%85%BC%EB%AC%B8%EB%A6%AC%EB%B7%B0.pdf)를 참고하세요.

## 참고 자료

- [Word2Vec: Skip-gram and CBOW](https://arxiv.org/abs/1301.3781)
- [Efficient Estimation of Word Representations in Vector Space](https://arxiv.org/abs/1301.3781)
