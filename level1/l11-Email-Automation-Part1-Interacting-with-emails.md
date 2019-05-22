# Lesson 11 - E-mail Automation Part 1 - Interacting with e-mails

## 이메일 인터렉션

* 이메일을 비즈니스 프로세스의 입력으로 사용
    * 데이터를 텍스트 형태로 받을 수 있다.
    * 이메일 제목, 본문, 첨부 파일 (Excel, PDF, ETC)

* 이메일을 비즈니스 프로세스의 출력으로 사용
    * 상태 업데이트를 보내는데 사용
    * 예외 발생.
    
## Email Activities

* SMTP (Simple Mail Transfer Protocol)
    * 메시지를 보내는 용도로만 사용되는 기본적인 프로토콜

* POP3 (Post office Protocol)
    * 지금은 거의 사용되지 않는 오래된 프로토콜
    * 메시지를 읽는데 사용된다.\
    * 대부분의 이메일 서버에서 지원된다.
    
* IMAP (Internet Message Access Protocol)
    * 메시지를 받는 용도로만 사용 되지만
    * 메시지를 읽은 상태로 표시하거나 폴더간 메세지를 이동하는 기능을 제공

* Exchange (마이크로소프트사의 엔터프라이즈 이메일 솔루션)
    * 메시지 주고받기
    * 폴더 이메일 이동
    * 이메일 삭제 등 제공
    
* OutLook
    * 데스크탑 애플리케이션의 API와 함께 작동
    * 액션에 컨텍스트가 있다.
    * 서버와 사용자를 설정할 필요가 없다.
    * 기존 OutLook 계정을 사용하도록 설계 돼 있다.
    
* Save Email Message Activity
* Save Attachments

## 이메일 가져 오기

* Get POP3 Mail Message
* Get Outlook Mail Messages
* Get IMAP Mail Messages
* GET Exchange Mail Messages
 
 > 특정 사서함 폴더에서 이메일을 가져 오고 읽지 않은 메시지만 가져오고 다시 처리되지 않도록 메시지를 읽은 상태로 표시하고
 > 수신 이메일 수를 제한하는 옵션, 서버 연결을 설정하기 위해 서버 주소와 포트가 일반적으로 필요 이메일 암호도 필요하다.
 
 > POP3, IMAP 에서는 유효성 경고가 표시됨. 연결 매개변수가 필요함
 > Outlook, Exchange는 표시되지 않음. 기본값과 자동검색을 사용하기 때문에 워크플로우 전반에 필요한 작업이 줄어듬.
 
 > 크레덴셜 에러의 경우 구글 설정에서 IMAP 허용 POP3허용 알지 못하는앱 접근 허용
 
 * Read Text File로 만들어진 템플릿을 읽어 메일의 제목과 본문은 완성할 수 있다.
 * 또한 String.Format을 통해 동적 콘텐츠를 만들수 있다.