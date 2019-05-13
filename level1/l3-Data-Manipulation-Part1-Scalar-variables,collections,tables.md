# 데이터 조작 및 변수

컨트롤 + K를 활용하여 액티비티의 속성 컨텍스트에 자동으로 형식에 맞는 변수를 생성할 수 있다,

## 변수 형식

* Scalar 변수 - 고정된 형식의 단일 값을 가짐.
    + Character, Boolean, Number, DateTime
    
* Collection - Array, List, Queue, String, Dict

* Tables - 행 인덱스와 컬럼이름으로 값에 액세스 할 수 있다.

* GenericValue - Strings, Booleans, Numbers, DateTImes

* Array - 고정된 크기를 가진다.
    + {"value1", "value2"}

* List - 요소를 추가/제거 하여 늘리거나 줄일 수 있다.
    + new List(of String) from {"value1", "value2"}
    + Invoke Method를 사용하여 요소를 추가 할 수 있다.
* 둘다 foreach 액티비티를 사용해 반복 가능 하다.

* Dictionary - 키/벨류 형태의 데이터 타입
    + new Dictionary(of String, String) from {{"key1","value1"},{"key2","value2"}}
    + 데이터 추가는 Assign을 이용하여 var("key3") = "value3"로 하면 된다.