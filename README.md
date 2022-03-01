# python openCV     
## 목차
0. [개요](#1.-개요)
18. [카드를 잘라서 파일로 저장하기](#-18.-카드를-잘라서-파일로-저장하기)


## 0. 개요
python으로 openCV 기초를 학습하였다. 이미지, 비디오를 불러오고 저장하는 방법부터, 이미지의 회전, grayscale로 변환, threshold(adaptive threshold), otsu algorithm, perspective transform을 직접 써보고 그 결과를 확인하였다. 


## 18 - 1. 카드를 잘라서 파일로 저장하기
poker 이미지에 있는 카드 이미지를 자르고 각도를 변환하여 각 카드 이미지를 저장하도록 하였다. 코드의 진행 순서는 아래와 같다.
1. 이미지를 불러온다.
2. grayscale, otsu algorithm으로 전처리를 거친다.
3. findContours로 윤곽선을 검출한다.
4. 카드를 찾은 경우에 해당 이미지를 crop하여 imshow로 출력함과 동시에 imwrite로 파일로 저장한다.



![카드 이미지](https://github.com/sanggon6107/python-opencv-practice/blob/master/card.png?raw=true)  
*↑카드 이미지*


![결과 이미지](https://github.com/sanggon6107/python-opencv-practice/blob/master/card_crop_1.png?raw=true)
*↑결과 이미지*


## 19. 동영상에서 사람 눈, 코 인식하기
mediapipe를 활용하여 동영상에서 사람 눈, 코를 인식하도록 하였다.
