# ESRGAN 모델 이용해보기
super resolution(초해상도) 모델 중 성능이 좋다고 알려진 ESRGAN 모델을 활용해 봅니다

## <img src="https://img.shields.io/badge/Tensorflow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white"> Tensorflow - ESRGAN
텐서플로우에서 제공하는 ESRGAN 모델 활용 방법에 대한 공식 홈페이지 글입니다.
https://www.tensorflow.org/hub/tutorials/image_enhancing?hl=ko

해당 글의 코드를 이용해 테스트를 진행했습니다.

## 텐서플로우 제공 이미지 결과
텐서플로우 글을 통해 아래와 같이 저화질 이미지를 고화질 이미지로 만들 수 있다고 합니다.
![image](https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/4a3ab55b-0f8c-4dfe-9018-297d974fd415)
![image](https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/d8279d09-6939-4203-96dc-e3e89df17000)

## 내가 사용한 이미지 결과
아이돌 그룹 에스파의 카리나 인스타를 통해 저화질 이미지를 구했습니다. 해당 이미지를 위 모델을 통해 고화질로 만든 결과입니다. 왼쪽이 원본이고 오른쪽이 모델을 통해 고화질로 수정된 이미지입니다.

<img width="350" alt="스크린샷 2024-01-10 143247" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/9f855c4b-9dc8-4e6f-9097-f945b3ac1233">
<img width="350" alt="스크린샷 2024-01-10 143247" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/b7e0e9eb-5b27-4258-b801-a726c2274278">

하지만 위 사진을 통해서는 실제로 화질이 좋아졌는지 크게 체감이 되지 않습니다. 그래서 사진을 확대해본 결과 약간의 개선은 있었다는 것을 알 수 있었습니다. 처음 나오는 이미지가 원본이고 후에 나오는 이미지가 고화질로 수정된 이미지입니다.

<img width="662" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/67aaebd4-7c78-4485-bbd3-bccc6d34b469">
<img width="651" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/1c86a19f-3477-4019-8642-8ce717d72102">

<img width="929" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/c0eb0305-1c76-461e-ac62-c366bdebf8f8">
<img width="859" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/1ea68c1c-97c5-478a-b958-7ec354b9ceb8">

## 이미지가 크게 달라지지 않는 이유 추정
텐서플로우에서 제공되는 기본 ESRGAN 모델은 128 x 128 크기의 이미지 패치에서 DIV2K 데이터세트(쌍입방 다운샘플링 이미지)에 훈련된 모델입니다. 그런데 제가 테스트하기 위해 사용한 에스파 카리나의 이미지는 500 x 700 크기 정도의 이미지입니다. 이렇게 더 큰 이미지에 대한 학습이 제대로 되지 않아서 위와 같은 일이 일어났을 것이라 추측했습니다.

그래서 더 큰 크기의 이미지를 활용해 추가 학습을 진행한 뒤, 결과를 비교해보겠습니다.






