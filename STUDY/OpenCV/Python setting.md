# Python setting

### visual studio code 에서 open CV 사용

1. cmd 창에 Open CV 라이브러리 설치 

```python
pip install opencv-contrib-python
```

1. vs code 에서 파일 생성
2. test.jpg 이미지 입력 후, 예제 실행

```python
//example code

import cv2

img_color = cv2.imread("test.jpg", cv2.IMREAD_COLOR)

if img_color is None:
	print("cannot read image file")
	exit(1)

cv2.namedWindow('Color')
cv2.imshow('Color', img_color)

cv2.waitKey(0)
cv2.destroyAllWindows()
```

1. ‘Run Python File in Terminal’ 을 통해 실행한다