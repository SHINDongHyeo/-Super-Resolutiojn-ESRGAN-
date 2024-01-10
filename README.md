# 1.ESRGAN 모델
super resolution(초해상도) 모델 중 성능이 좋다고 알려진 ESRGAN 모델을 활용해 봅니다

## <img src="https://img.shields.io/badge/Tensorflow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white"> Tensorflow
텐서플로우에서 제공하는 ESRGAN 모델 활용 방법에 대한 공식 홈페이지 글입니다.
https://www.tensorflow.org/hub/tutorials/image_enhancing?hl=ko

해당 글의 코드를 이용해 테스트를 진행했습니다.

## ✅텐서플로우 제공 이미지 결과
텐서플로우 글을 통해 아래와 같이 저화질 이미지를 고화질 이미지로 만들 수 있다고 합니다.
![image](https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/4a3ab55b-0f8c-4dfe-9018-297d974fd415)
![image](https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/d8279d09-6939-4203-96dc-e3e89df17000)

## ☑️내가 사용한 이미지 결과
아이돌 그룹 에스파의 카리나 인스타를 통해 저화질 이미지를 구했습니다. 해당 이미지를 위 모델을 통해 고화질로 만든 결과입니다. 왼쪽이 원본이고 오른쪽이 모델을 통해 고화질로 수정된 이미지입니다.

<img width="350" alt="스크린샷 2024-01-10 143247" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/9f855c4b-9dc8-4e6f-9097-f945b3ac1233">
<img width="350" alt="스크린샷 2024-01-10 143247" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/b7e0e9eb-5b27-4258-b801-a726c2274278">

하지만 위 사진을 통해서는 실제로 화질이 좋아졌는지 크게 체감이 되지 않습니다. 그래서 사진을 확대해본 결과 약간의 개선은 있었다는 것을 알 수 있었습니다. 처음 나오는 이미지가 원본이고 후에 나오는 이미지가 고화질로 수정된 이미지입니다.

<img width="662" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/67aaebd4-7c78-4485-bbd3-bccc6d34b469">
<img width="651" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/1c86a19f-3477-4019-8642-8ce717d72102">

<img width="929" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/c0eb0305-1c76-461e-ac62-c366bdebf8f8">
<img width="859" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/1ea68c1c-97c5-478a-b958-7ec354b9ceb8">

# 2. Real-ESRGAN 모델
ESRGAn보다 성능이 더 좋다고 알려진 모델을 찾아서 해당 모델도 사용해보았습니다.

## <img src="https://img.shields.io/badge/Github-000000?style=flat-square&logo=github&logoColor=white"> Github
해당 모델에 관한 자세한 설명이 담긴 github 주소입니다.
https://github.com/xinntao/Real-ESRGAN?tab=readme-ov-file#python-script


## ✅깃허브 제공 이미지 결과
깃허브 readme에 작성된 코드를 통해 이미지와 모델을 다운받아 확인한 결과입니다. 왼쪽이 원본 이미지고 오른쪽이 모델을 통해 고화질로 수정된 이미지입니다.

<img width="433" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/c265dd12-9b77-4d51-9155-e9cd59fef9c4">
<img width="432" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/bb89c257-cbaf-4274-87bd-e8b292423a03">
<img width="439" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/8add4f2f-5f15-4702-8567-28f378fed9e3">
<img width="434" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/62c5d06b-6bdd-405b-9d48-6558b43cefed">



## ☑️내가 사용한 이미지 결과
위에서 ESRGAN을 통해 테스트한 카리나 사진에서는 크게 화질이 좋아짐을 체감할 수 없었습니다. 하지만 Real-ESRGAN 모델을 통해서는 화질이 눈에 띄게 좋아짐을 확인할 수 있었습니다. 처음 나오는 이미지가 원본이고 후에 나오는 이미지가 고화질로 수정된 이미지입니다.

<img width="350" alt="karina" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/2dcab9ec-c710-44c8-82ba-8ab8a90f9376">
<img width="350" alt="karina" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/3038d1b9-a9c5-404c-8157-221c58ca21e1">

<img width="662" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/67aaebd4-7c78-4485-bbd3-bccc6d34b469">
<img width="453" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/0c905e49-7522-4b1a-a21e-a97abe0b9abf">

<img width="929" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/c0eb0305-1c76-461e-ac62-c366bdebf8f8">
<img width="897" alt="image" src="https://github.com/SHINDongHyeo/ESRGAN-super-resolution-model/assets/96512568/db1f235e-81a8-4f91-9d52-07cafd9c5143">

엄청 화질이 좋아졌습니다!!!😲

원래 성능이 이렇게 좋을지 모르고 미세 조정을 통해 더 높은 성능의 모델을 만들어 보려고 했으나, 이 정도 결과물이라면 따로 미세 조정은 필요 없을 것 같습니다...

