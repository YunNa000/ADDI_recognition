# **감정 인식 모델**

이 프로젝트는 MMA Facial Expression 데이터셋을 사용하여 감정을 인식하는 딥러닝 모델을 개발하고, 이를 Android 앱에 통합하여 실시간으로 감정을 분석하는 기능을 구현합니다. MobileNetV2 아키텍처를 기반으로 한 모델 학습 과정과 Android Studio를 사용한 앱 개발 과정이 포함됩니다.

이를 통해  자폐아동의 표정을 구분하고 (행복, 슬픔, 화남, 혐오, 놀람) 피드백 메세지를 통해 적절한 학습을 할 수 있도록 도와줍니다.


## **프로젝트 구성**

- **데이터 수집**: [MMA Facial Expression 데이터셋](https://www.kaggle.com/datasets/mahmoudima/mma-facial-expression) 사용
- **모델 학습**: [Kaggle 노트북](https://www.kaggle.com/code/pramod722445/notebook73b2680e27/notebook) 참조
- **모델 다운로드**: [Kaggle 모델 링크](https://www.kaggle.com/datasets/pramod722445/model300)
- **안드로이드 앱 개발**: 실시간 감정 인식을 위한 Android Studio 사용
  

## **시작하기**

### **사전 요구사항**

- Python 3.6 이상
- TensorFlow 2.x
- Android Studio Dolphin | 2021.3.1
- Kaggle 계정


### **설치**

1. 필요한 Python 라이브러리를 설치합니다:
    
    ```bash
    bashCopy code
    pip install tensorflow kaggle
    
    ```
    
2. Kaggle API를 사용하여 필요한 데이터셋과 모델을 다운로드합니다:
    
    ```bash
    bashCopy code
    kaggle datasets download -d mahmoudima/mma-facial-expression
    kaggle datasets download -d pramod722445/model300
    
    ```
    
3. 다운로드한 데이터셋과 모델을 적절한 작업 디렉토리로 이동합니다.

### **모델 학습**

학습 과정에 대한 자세한 내용은 [이 Kaggle 노트북](https://www.kaggle.com/code/pramod722445/notebook73b2680e27/notebook)을 참고하세요. 노트북에는 데이터 전처리, 모델 구성, 학습 및 평가 과정이 상세히 설명되어 있습니다. 


### **앱 UI**
<img width="527" alt="image" src="https://github.com/ADDIcreamo/ADDI_recognition/assets/54527982/75afb0b4-a1d3-4c8c-b373-10a20bfee9e4">
<img width="524" alt="image" src="https://github.com/ADDIcreamo/ADDI_recognition/assets/54527982/7527b6ee-467c-4e3c-be41-e262cc04dadf">

### **Android Studio Project Tree**
```bash
C:.
├─assets
├─java
│  └─com
│      └─example
│          └─imagepro
├─jnilibs
│  ├─arm64-v8a
│  ├─armeabi
│  ├─armeabi-v7a
│  ├─mips
│  ├─mips64
│  ├─x86
│  └─x86_64
└─res
    ├─drawable
    ├─drawable-v24
    ├─layout
    ├─mipmap-anydpi-v26
    ├─mipmap-hdpi
    ├─mipmap-mdpi
    ├─mipmap-xhdpi
    ├─mipmap-xxhdpi
    ├─mipmap-xxxhdpi
    ├─raw
    ├─values
    └─values-night
```

### **작동 화면**
<img width="563" alt="image" src="https://github.com/ADDIcreamo/ADDI_recognition/assets/54527982/4620afd6-8ee7-4f44-a690-874eadcea8b6">

<img width="603" alt="image" src="https://github.com/ADDIcreamo/ADDI_recognition/assets/54527982/6205858b-24dd-4802-b4f5-b0987fc249fe">

