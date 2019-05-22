# Lesson 12 - Debugging and Exceptions Part 3 - Catching errors

## Try-Catch
*Try, Catch, Finally로 구성
* Try
    + required
    + 오류가 발생할수 있는 액션을 넣음
* Catch
    + required
    + 오류가 발생하면 실행할 액션을 넣음
    + 여러개의 Exception을 Catch할 수 있음
* Finally
    + optional
    + 무조건 실행될 액션을 넣음.

* 오류 메시지의 Exception Type필드를 보면 Exception의 종류를 파악할 수 있다.
* Rethrow액션으로 워크플로우를 중지 할 수 있다.

## Invoke workflow file

* 워크 플로우를 모듈화 하여 다른 곳에 사용 할 수 있다.