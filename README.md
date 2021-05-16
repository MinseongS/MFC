# MFC

## MFC 실습
### RAW 파일을 불러오고 다양한 방법으로 변환해 본다.
***
### 기능
#### - OnOpenDocument : RAW 파일을 열기 위해 파일을 불러옴
#### - OnSaveDocument : 변환한 파일을 RAW파일로 저장함.
#### - OnDrawDocument : 변환한 이미지와 원본 이미지를 둘 다 출력.
#### - OnDownSampling : Dialog1 에서 Rate를 받아 DownSampling.
##### └ Dialog1 : 1~255 범위의 int 값을 받음.
#### - OnUpSampling : Dialog1 에서 Rate를 받아 UpSampling.(선형보간으로 구현)
##### └ Dialog1 : 1~255 범위의 int 값을 받음.
#### - OnQuantization : Dialog2 에서 받은 수로 양자화의 단계를 결정하여 변형.
##### └ Dialog2 : 1~8 범위의 int 값을 받음.
#### - OnAndOperate : 상수값을 받아 전체 데이터에 합 연산.
##### └ Dialog1 : 1~255 범위의 int 값을 받음.
#### - OnOrOperate
#### - OnXorOperate
#### - OnGammaTransform
#### - OnNegaTransform
#### - OnBinarization
#### - OnStressTransform
#### - OnHistoStretch
#### - OnEndInSearch
#### - OnHistogram
#### - OnHistoEqual
#### - OnHistoSpec
#### - OnEmbossing
#### - OnBlurr
#### - OnGaussianFilter
#### - OnSharpening
#### - OnHpfSharp
#### - OnLpfSharp
#### - OnDiffOperatorHor
#### - OnHomogenOperator
#### - OnLaplacian
#### - OnNearest
#### - OnBilinear
#### - OnMedianSub
#### - OnMeanSub
#### - OnTranslation
#### - OnMirrorHor
#### - OnMirrorVer
#### - OnRotation
#### - OnFrameSum
#### - OnFrameSub
#### - OnFrameMul
#### - OnFrameDiv
#### - OnFrameAnd
#### - OnFrameOr
#### - OnFrameComb
#### - OnBinaryErosion
#### - OnBinaryDilation
#### - OnGrayErosion
#### - OnGrayDilation
#### - OnLowPassFilter
#### - OnHighPassFilter
#### - OnMeanFilter
#### - OnMedianFilter
#### - OnMaxFilter
#### - OnMinFilter
#### - OnFft2d
#### - OnIfft2d
#### - OnLpfFrequency
#### - OnHpfFrequency
