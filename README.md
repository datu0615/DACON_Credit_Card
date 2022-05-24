# DACON_Credit_Card
![20220524_130938](https://user-images.githubusercontent.com/84311270/169983071-07e23b39-bfec-41e8-af4e-809517843ab8.png)
신용카드 사용자 데이터를 보고 사용자의 대금 연체 정도를 예측하는 알고리즘 개발 

## Dataset
train.csv  
train 데이터 : 신용카드 사용자들의 개인 신상정보  
credit 열 포함  
train.shape : (26457, 20)  

test.csv  
test 데이터 : 신용카드 사용자들의 개인 신상정보  
credit 열 미포함  
test.shape : (10000, 19)  

sample_submission.csv  
정답 제출 파일  
sample_submission.shape :(10000, 4)  

## Model
다양한 파생변수 생성 및 LightGBM을 활용하여 학습을 진행. Optuna를 사용하여 hyper-parameter를 최적화.

## Results
Public Score : 0.67914, Private Score : 0.66289로 최종 13등으로 마무리.
![20220524_130958](https://user-images.githubusercontent.com/84311270/169983428-b9e5b817-daa4-41d1-90df-2d032d0e382b.png)
