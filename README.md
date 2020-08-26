# QuickDraw_Canvas

구글에서 만든 온라인 게임 QuickDraw 의 데이터 셋을 이용한 프로그램입니다.

플레이어가 사물이나 개념에 대한 그림을 그리면 인공신경망 인공지능을 사용하여 해당 낙서가 표현한 바를 텍스트와 이미지 그리고 음성으로 대답합니다.

이 프로젝트는 [gautamkumarjaiswal](https://github.com/gautamkumarjaiswal/QucikDraw) 의 프로젝트를 참고하여 만든 프로젝트 입니다.

------

It is a program that uses the data set of the online game QuickDraw made by Google.

When the player draws a picture of an object or concept, the artificial neural network uses artificial intelligence to respond with text, images, and voice to what the doodle expresses.

This project was created by referring to the project of [gautamkumarjaiswal](https://github.com/gautamkumarjaiswal/QucikDraw)

# 사용법 manual

  1. data 폴더에 원하는 [numpy bitmap 데이터](https://console.cloud.google.com/storage/browser/quickdraw_dataset/full/numpy_bitmap) 를 추가해줍니다.

  2. readDataset.py 를 실행합니다.
  
  3. trainModel.py 를 실행합니다. 시간이 좀 걸릴 수 있습니다.
  
  4. imagePredict.py 를 실행합니다.
  
    1. 그림을 그립니다.
    
    2. predict 를 눌러주시면, 조금의 시간이 걸린 후 사용자가 그린 그림의 이름을 답합니다.
    3. clear 를 눌러주시면, 캔버스를 지워줍니다. - 2020/8/19 지워도 더미 데이터가 남는 문제 발생
    4. save 를 눌러주시면, 자기가 그린 그림을 저장합니다.
    5. voice 를 눌러주시면, 도출한 답에 대해 음성으로 출력해줍니다. - 2020/8/19 코드는 문제가 없고 사용자가 mp3를 추가해서 사용해야 합니다.
  
  ------
  
  1. Keep downloaded [dataset](https://console.cloud.google.com/storage/browser/quickdraw_dataset/full/numpy_bitmap) in folder 'data'.

  2. Run readDataset.py to load dataset.

  3. Use trainModel.py to train CNN model, This may take some time depend on configuration of system.

  4. Run imagePredict.py to test developed model.
  
    1. Draw a picture.
    
    2. If you preess predict Button, The program will answer by guessing the picture you drew. Instead, it takes a little time.
    3. If you preess clear Button, The program will clear the Canvas - 2020/8/19 An error has occurred that leaves dummy data.
    4. If you preess save Button, The program will save your drawing.
    5. If you preess voice Button, The program responds with a voice, guessing the picture you drew.
    
  
# 이미지

## 시작 이미지

<img src="https://user-images.githubusercontent.com/31675804/90640752-58f43980-e26b-11ea-8a88-33d1861ed9ca.PNG" width="90%"></img>

## 그림 인식

<img src="https://user-images.githubusercontent.com/31675804/90640961-9a84e480-e26b-11ea-9dea-37d236d5e3ec.PNG" width="90%"></img>

## 비고
  * runWebCam.py 파일은 [gautamkumarjaiswal](https://github.com/gautamkumarjaiswal/QucikDraw) 님의 프로젝트의 파일로, 코드의 해석에 어려움이 있었기에 따로 한글로 주석을 추가했습니다.
  
  * 코드 실행에 어려움이 있으시면 [gautamkumarjaiswal](https://github.com/gautamkumarjaiswal/QucikDraw) 님의 README 를 읽고 runWebCam.py 대신 imagePredict.py 를 실행해주세요.