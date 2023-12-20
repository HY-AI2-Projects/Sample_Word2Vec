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

* Word2Vec을 소개한 Efficient estimation of word representations in vector space 논문에 대한 추가적인 내용은 [논문요약자료](https://github.com/HY-AI2-Projects/Word2Vec/blob/main/Word2Vec_%EB%85%BC%EB%AC%B8%EB%A6%AC%EB%B7%B0.pdf)를 참고하세요.

## 참고 자료

- [Word2Vec: Skip-gram and CBOW](https://arxiv.org/abs/1301.3781)
- [Efficient Estimation of Word Representations in Vector Space](https://arxiv.org/abs/1301.3781)

## 영화 리뷰를 이용한 Word2Vec 실습

* Word2Vec 파이썬 스크립트는 Word2Vec 및 t-SNE을 사용하여 한국어 영화 리뷰 데이터를 자연어 처리하고 텍스트 데이터를 시각화하는 작업을 수행합니다.

## 사용된 라이브러리

- `pandas`
- `numpy`
- `matplotlib`
- `re`
- `urllib.request`
- `konlpy`
- `tensorflow.keras.preprocessing.text.Tokenizer`
- `gensim.models.Word2Vec`
- `sklearn.decomposition.PCA`
- `sklearn.manifold.TSNE`

## 주요 기능

1. **데이터 로딩 및 전처리**: NSMC에서 제공하는 한국어 영화 리뷰 데이터를 불러오고 전처리합니다.

2. **텍스트 전처리 및 토큰화**: Okt 형태소 분석기를 사용하여 텍스트를 토큰화하고 불용어를 제거합니다.

3. **Word2Vec 모델 학습**: Gensim을 사용하여 토큰화된 문장에 대한 Word2Vec 모델을 학습합니다.

4. **PCA를 사용한 2D 시각화**: Word2Vec에서 얻은 단어 벡터를 2D로 시각화합니다.

5. **t-SNE를 사용한 2D 시각화**: t-SNE 알고리즘을 활용하여 단어 임베딩을 또 다른 2D 시각화로 제공합니다.

6. **플로팅 및 시각화**: Matplotlib을 사용하여 시각화된 결과를 플로팅하고 각 포인트에 대한 레이블을 표시합니다.

7. **모델 학습 결과 해석**: PCA 및 t-SNE의 시각화를 통해, 학습된 Word2Vec 모델이 단어 간 의미적 유사성을 잘 포착하고 있는지 확인할 수 있습니다.


## 참고 사항

- 이 프로젝트는 Gensim, scikit-learn, Konlpy 등 다양한 라이브러리를 활용하여 구현되었습니다.
- 한국어 자연어 처리에 대한 이해가 필요한 독자를 위해 코드에 주석을 추가하였습니다.
- 추가적인 데이터 전처리나 모델 튜닝을 수행하고자 하는 경우, 코드를 수정하여 원하는 대로 확장할 수 있습니다.

## 기여 및 문의사항

- 이 프로젝트에 대한 기여는 언제나 환영합니다. 버그를 찾거나 새로운 기능을 제안하려면 GitHub 저장소에 이슈를 작성해주세요.
- 추가적인 도움이 필요하거나 의문사항이 있으면 이 문서 하단에 댓글을 남겨주세요.
이 코드의 주요 목적은 한국어 영화 리뷰 데이터를 활용하여 단어 간의 관계를 시각적으로 이해하는 것입니다. Word2Vec을 사용하여 단어를 벡터로 표현하고, PCA 및 t-SNE를 사용하여 벡터를 2D 공간으로 투영하여 시각화하는 것은 데이터의 패턴과 관계를 더 잘 이해할 수 있도록 도와줍니다.
