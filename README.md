# MFC

## MFC 실습
### RAW 파일을 불러오고 다양한 방법으로 변환해 본다.
***
### 기능
#### - OnOpenDocument : RAW 파일을 열기 위해 파일을 불러옴
#### - OnSaveDocument : 변환한 파일을 RAW파일로 저장함
#### - OnDrawDocument : 변환한 이미지와 원본 이미지를 둘 다 출력
#### - OnDownSampling : Dialog1 에서 Rate를 받아 DownSampling
##### └ CConstantDlg : 1~255 범위의 int 값을 받음
#### - OnUpSampling : Dialog1 에서 Rate를 받아 UpSampling(선형보간으로 구현)
##### └ CConstantDlg : 1~255 범위의 int 값을 받음
#### - OnQuantization : Dialog2 에서 받은 수로 양자화의 단계를 결정하여 변형
##### └ CQuantization : 1~8 범위의 int 값을 받음
#### - OnSumOperate : 상수값을 받아 전체 데이터에 합 연산
##### └ CConstantDlg : 1~255 범위의 int 값을 받음
#### - OnSubOperate : 상수값을 받아 전체 데이터에 뺄셈 연산
##### └ CConstantDlg : 1~255 범위의 int 값을 받음
#### - OnMulOperate : 상수값을 받아 전체 데이터에 곱 연산
##### └ CConstantDlg : 1~255 범위의 int 값을 받음
#### - OnDivOperate : 상수값을 받아 전체 데이터에 나눗셈 연산
##### └ CConstantDlg : 1~255 범위의 int 값을 받음
#### - OnAndOperate : 상수값을 받아 전체 데이터에 AND 연산
##### └ CConstantDlg : 1~255 범위의 int 값을 받음
#### - OnOrOperate : 상수값을 받아 전체 데이터에 OR 연산
##### └ CConstantDlg : 1~255 범위의 int 값을 받음
#### - OnXorOperate : 상수값을 받아 전체 데이터에 XOR 연산
##### └ CConstantDlg : 1~255 범위의 int 값을 받음
#### - OnGammaTransform : 실수값을 받아 전체 데이터에 Gamma 변환
##### └ CGammaDlg : 0~2.0 범위의 float 값을 받음
#### - OnNegaTransform : 255 - inputImage를 통해 반전
#### - OnBinarization : 기준값으로 데이터 이진화
##### └ CConstantDlg : 1~255 범위의 int 기준값을 받음
#### - OnStressTransform : 범위 내 값을 모두 흰색으로 변환
##### └CStressTransformDlg : 1~255 범위의 int 기준값을 두개 받음
#### - OnHistoStretch : 최대, 최소 기준으로 히스토그램 스트레칭
#### - OnEndInSearch : 최대, 최소을 임계값으로 사용한 후 스트레칭
#### - OnHistogram : 이미지의 히스토그램을 보여줌
#### - OnHistoEqual : 이미지 평활화(데이터가 밀집되어있는 곳을 집중적으로 스트레칭)
#### - OnHistoSpec : 다른 이미지의 히스토그램과 비슷하게 만들어줌
#### - OnEmbossing : 엠보싱 변환
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
