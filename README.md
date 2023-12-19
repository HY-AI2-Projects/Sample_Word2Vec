Word2Vec이란?
Word2Vec은 단어를 벡터로 표현하는 자연어 처리(Natural Language Processing, NLP) 기술 중 하나로, 단어 간 의미적 유사성을 수치적으로 나타냅니다. 이 기술은 단어들을 연속적인 공간에 투영하여 단어 간의 관계를 이해하고, 단어 벡터 간의 거리를 통해 의미적 유사성을 측정합니다.

Word Embedding
Word2Vec은 단어 임베딩의 한 형태로, 단어를 고차원 벡터로 매핑하는 작업입니다. 임베딩된 단어 벡터는 단어의 의미와 관련된 정보를 포함하고 있으며, 유사한 의미를 가진 단어들은 벡터 공간에서 서로 가깝게 위치합니다.

CBOW (Continuous Bag of Words) 모델
CBOW 모델은 주변 단어들의 임베딩을 이용하여 특정 단어를 예측하는 모델입니다. 주변 단어들의 평균 벡터를 입력으로 사용하고, 이를 통해 대상 단어를 예측합니다.

Skip-gram 모델
Skip-gram 모델은 특정 단어를 입력으로 받아 주변 단어들을 예측하는 모델입니다. 입력 단어를 이용해 주변 단어들을 하나씩 예측하는 방식으로 학습됩니다.

학습 과정
Word2Vec 모델은 대량의 텍스트 데이터를 사용하여 단어 간의 관계를 학습합니다. 모델이 학습되면 단어 간 유사성 및 의미적 관계를 캡처하는 벡터 표현이 얻어집니다.

예제
이 저장소에는 Gensim 라이브러리를 사용하여 Word2Vec 모델을 훈련하는 간단한 예제가 포함되어 있습니다. 자세한 사용법은 여기를 참조하세요.

참고 자료
Word2Vec: Skip-gram and CBOW
Efficient Estimation of Word Representations in Vector Space
