# 데이터 결합

* 다양한 데이터를 텍스트로 결합해야하는 경우도 생긴다.
* String을 결합 하거나 String.Format을 사용

## 다양한 데이터 연결

* 모든 데이터 형식에는 기본적으로 ToString메소드가 있다.
* 이를 통해 텍스트로의 연결및 결합을 하면 된다

## Format

* String,Format("Hello {0} {1:MMMM yyyy}", "world", Now)의 형태로 사용

## String Methods

* Contains
    + 문자열 포함 확인
    + filePath.Contains(".")
    + True
* EndsWIth/StartsWith
    + 문자열 시작이나 끝 확인
    + filePath.EndsWith(".txt")
    + True
* Replace
    + 문자열에 동일한 문자열 변경
    + filePath.Replace("/","\")
    + "DD\DD" -> "DD/DD"
* Split
    + 문자열을 기준 문자로 자름
    + filePath.Split("/".ToCharArray)
    + {"DD", "DD"}
* Substring
    + Index이후부터 문자열을 자름
    + filePath.Substring(2)
    + "DD"
* ToLower/ToUpper
    + 대문자/소문자로 변경
    + filePath.ToLower
    + "dd/dd"
* Trim
    + 공백 문자 제거
    + random.Trim
    + "ASD"
    
## Tables

* csv파일을 읽을때에는 ReadCsv를 사용한다.
    + DataRow[] 사용하여 row를 for each로 가져 올 수 있다.
    