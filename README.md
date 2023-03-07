# cv_project
## 주제
- 수천개 이상의 작은 이미지로 큰 하나의 이미지 만들기(Collage Mosaic Generator)
- ![원본](target.jpg)
- ![821](mosaic(821).jpeg)

## WBS
|항목|2023-03-07(화)|2023-03-08(수)|
|:-|:-:|:-:|
|레퍼런스 서치|완료||
|프로젝트 진행|완료||
|결론 도출|완료||
|보완||진행중|

## 진행사항
1. 타겟 이미지 선정(유튜브 썸네일)
2. 타일 이미지(샘플 영상에서 원하는 프레임 단위로 추출) 생성
3. Pillow 라이브러리 에서 OpenCV 라이브러리 사용하는 것으로 코드 수정(진행중)

## 결론
1. Pillow의 Image.new() 에 해당하는 cv2의 기능이 없는것으로 생각됨
2. 타겟 이미지를 50x50 픽셀 단위로 쪼갠다음, 해당 단위의 color를 얻어냄
3. 생성된 타일 이미지의 color 값을 토대로 쪼개진 타겟 이미지의 color 근사치를 확인
4. 유사한 이미지 값으로 새롭게 생성

## 참고 레퍼런스
- [Top 25 Computer Vision Project Ideas for 2022](https://data-flair.training/blogs/computer-vision-project-ideas/)
- [mosaic github](https://github.com/codebox/mosaic)
- [동영상 프레임 초단위 저장/캡처](https://thinking-developer.tistory.com/61)
- [cv2와 PIL 라이브러리를 활용하여 이미지 다루기](https://soyoung-new-challenge.tistory.com/112)
- [Python OpenCV 와 PIL 의 상호 변환](https://www.zinnunkebi.com/python-opencv-pil-convert/)
- [pil, opencv 비교](https://blog.naver.com/PostView.naver?blogId=nkj2001&logNo=222764410613&categoryNo=0&parentCategoryNo=62&viewDate=&currentPage=1&postListTopCurrentPage=1&from=search)