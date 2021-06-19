# Python 실습보고서 #1

## 사용 기술

### 실습환경

- Python 3.7.6

### 사용 라이브러리

- `scipy.ndimage`: Multi-dimensional image processing
- `numpy`: It provides a high-performance multidimensional array object
- `matplotlib.pyplot`: It provides a MATLAB-like way of plotting.

## 이진화(thresholding)

- 이진화(thresholding)의 임계값을 바꾸면서 출력 영상의 변화를 관찰
- Thresholding 기법은 영상에서 각각의 픽셀들의 값을 특정한 임계값 보다 낮은 픽셀은 검정색(0)으로, 임계값과 같거나 높은 픽셀은 흰색(255)으로 바꾸는 기술.

## 감마 보정법(Gamma correction)

- 감마 보정을 적용하여 입력과 결과 영상을 비교
- 감마 보정법은 감마의 역수를 최종 출력 이미지에 적용하는 기술. 역 감마곡선을 선형 출력 색상에 곱해 빛의 강도를 비선형적으로 변형하는 방식으로 영상의 밝기를 조절할 수 있다.

## 평균 필터링

- 평균 필터의 마스크 크기를 바꿔가면서 필터링하고, 결과를 관찰
- 공간상의 평균 필터링이란, 영상 신호에 대하여 공간 영역(Spatial Domain)에서의 필터 처리를 의미한다. 하나의 픽셀값을 구하기위해 주변 픽셀값들을 이용하는 방식으로 필터링되고 중앙에 처리값이 저장되어 마스크는 반드시 홀수\*홀수 형태를 가져야함.

## contrast stretching

- Contrast stretching는 명암비를 늘려 영상 화질을 향상시키는 기술.
