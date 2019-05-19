# Lesson 7 - Image and Text Automation Part 3 - Image-based automation: Retrieve Information

## 정보 얻기
* 가상머신에서 정보를 얻기 위해 두가지 방법이 있다.
    + Select & Copy
        + 간단
        + 선택가능한 텍스트에만 사용 가능
        + 활성 텍스트 필드에서만 액션이 수행됨.
    * Scrape Relative
        + 스크래핑할 영역을 지정하여 정보를 얻음
        + Scale값을 조정하여 더 정확한 정보를 획득
        + 앵커 이미지를 찾으면 선택한 앵커 항목과 일치하는 영역이 실제 결과가 됨.
        * 앵커 이미지를 기준으로 지정된 영역을 계산함.
        + 그리고 해당 영역의 콘텐츠를 얻음. GET OCR Text를 사용하여.
        + 클리핑.