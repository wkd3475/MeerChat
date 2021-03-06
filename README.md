# MeerChat
Chatting Shell with Golang

## 하나 목표
각자 *브랜치*를 파서 작동하는 채팅(서버) 구현하기.
- 다음모임때 코드 리뷰를 해서 채팅서버 통합하기.
- P2P던, 채팅방만들기던 메세지를 주고받을 수 있어야 함.
- 터미널이던 웹이던 뭐든 작동해야함.

다음 모임 날짜
- 21일 화요일 저녁 6시에 모여서 같이 밥먹고 합시다.

## 둘 목표
Shell CUI 구현하기. shell 명령어 되면서 상단/우측/좌측/하단/ 임의의 그림이 보이게
- 다다음모임때 코드 리뷰해서 통합하기


### 기능 정리
참고자료
https://github.com/faroyam/golang-p2p-chat/blob/master/chat.go

select 참고 자료
https://hamait.tistory.com/1017

- 노드
    - [x] 하나의 노드 안에 서버와 클라이언트가 동시에 존재하게 만들기
    - [ ] 다른 서버에 연결 요청
        - [x] 단순히 연결하는 것만 구현되어 있음
    - [ ] 연결된 서버 정보 출력

- 채팅
    - [x] 문자 보내기
    - [x] 받은 문자 출력

- 채팅방 (채팅방은 우선 고려X)
    - [ ] 채팅방 추가
    - [ ] 채팅방 삭제
    - [ ] 채팅방 수정
    - [ ] 채팅방 출력
    - [ ] 채팅방 참가
    - [ ] 채팅방 탈퇴
    - [ ] 채팅방 초대

- docker
    1. docker build -t meerchat .
    2. sudo docker run -it -p 7000:7000 --rm --name meerchat1 meerchat
    3. sudo docker run -it -p 8000:7000 --rm --name meerchat2 meerchat
    