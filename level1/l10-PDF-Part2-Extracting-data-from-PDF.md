# Lesson 10 - PDF Part 1 - Extracting data from PDF

## 설치

* Activity창에 PDF를 검색했는데 없을 경우 패키지 매니저에서 UiPath.PDF.Activities를 찾아 설치 하자

## PDF

* PDF파일에는 텍스트와 이미지가 포함 될 수 있다.
* 텍스트로 보이지만 이미지인 경우도 있다.
* 식별방법중 기본은 선택하면 텍스트와 이미지는 선택영역이 다르게 나타난다.

## 2가지 큰 범주

* 큰 텍스트 블록이나 전체 문서에 관한것
    * Read PDF Text를 사용하여 전체 PDF문서 또는 페이지를 읽을수 있다.
    * Read PDF with OCR을 사용하여 이미지로 된 텍스트를 읽을 수 있다.
    * 두 방식다 백그라운드에서 동작 가능 하다.
    
* PDF파일에서 특정 텍스트 항목을 추출 하기 위한 것. 네임, 제품, 인보이스 금액 등
    * screen scraping tool 을 사용한다.

## 정확도

* 좋은 해상도와 글꼴이 있어야 이미지 텍스트 분석이 잘 된다.