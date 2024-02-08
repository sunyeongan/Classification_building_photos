# 한림대학교 건물 사진 분류

## 프로젝트 소개 
- 한림대학교 5개 건물 (공학관, 일송아트홀, 산학협력관, 본부별관, CLC) 사진을 촬영/수집하고 해당 건물 사진을 분류하는 딥러닝 모델 개발

## 데이터셋 수집 & 전처리 소개 
![image](https://github.com/sunyeongan/Classification_building_photos/assets/44018024/ff496332-c415-4b5a-993d-2bfcb7bf878e)
- 각 건물 사진 약 100장 정도를 갤럭시, 아이폰으로 수집함.
- 아이폰에서 찍은 사진의 경우, 이미지 확장자가 .HEIC이므로 별도로 확장자를 JPG로 바꾸는 작업이 필요.(https://seonybob3210.tistory.com/12)
- 이미지 이름은 "C+건물클래스+인덱스+.jpg"로 설정.
- train dataset 320, valid dataset 80, test dataset 100으로 구성 
## 딥러닝 모델 구성 
- pre-trained vgg16 모델 + fully connected 2 layer로 구성
- ![image](https://github.com/sunyeongan/Classification_building_photos/assets/44018024/84f828b1-c5f6-4ec5-8fc4-7dd1e6f908c3)
## 학습
- Model : vgg16
- epoch : 10
- optimizer : Adam
- learning rate : 1e-5
- env : colab
## 테스트 성능 
- loss : 0.968388
- acc : 0.73
- ![image](https://github.com/sunyeongan/Classification_building_photos/assets/44018024/e2b2e55e-93eb-4cf4-974a-77251306aa3f)

