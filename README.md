# QuickDraw_Canvas

구글에서 만든 온라인 게임 QuickDraw 의 데이터 셋을 이용한 프로그램입니다.

플레이어가 사물이나 개념에 대한 그림을 그리면 인공신경망 인공지능을 사용하여 해당 낙서가 표현한 바를 텍스트와 이미지 그리고 음성으로 대답합니다.

이 프로젝트는 [gautamkumarjaiswal](https://github.com/gautamkumarjaiswal/QucikDraw) 의 프로젝트를 참고하여 만든 프로젝트 입니다.

# 사용법

  1. data 폴더에 원하는 [numpy bitmap 데이터](https://console.cloud.google.com/storage/browser/quickdraw_dataset/full/numpy_bitmap) 를 추가해줍니다.

  2. readDataset.py 를 실행합니다.
  
  3. trainModel.py 를 실행합니다. 시간이 좀 걸릴 수 있습니다.
  
  4. imagePredict.py 를 실행합니다.
  
# 이미지

## 시작 이미지

<img src="https://user-images.githubusercontent.com/31675804/90640752-58f43980-e26b-11ea-8a88-33d1861ed9ca.PNG" width="90%"></img>

## 그림 인식

<img src="https://user-images.githubusercontent.com/31675804/90640961-9a84e480-e26b-11ea-9dea-37d236d5e3ec.PNG" width="90%"></img>
