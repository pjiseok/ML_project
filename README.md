### <목적> - 회사 파산 여부 파악하기

1. 파산 여부 파악 - 분류
2. 파산에 어떤 특성이 영향이 있는가 - 상관관계분석 (부채,순이익)
3. pca로 차원축소 -연관있는것끼리 묶어보자 

전처리
- 낮은특성중요도 없애기

테스트
- 데이터 밖 진짜 파산 회사 데이터가져오기


파일명
train_data : 전체 데이터에서 80% 분리한 트레인 데이터
test_data : 전체 데이터에서 20%차지하는 테스트데이터 (모델학습x)

train_data_reduced : 0.01미만의 낮은 특성중요도 제거한 트레인데이터 (54개 특성제거)
test_data_reduced : 낮은 특성중요도 제거한 테스트 데이터
low_importance_features : 제거한 54개의 특성

### <최종>
- 언더샘플링 기법을 사용함
- 최적의 파라미터를 찾아서 recall(재현율)을 높힘
