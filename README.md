# Spring 항해 개인 과제 
 

![스크린샷 2022-12-08 오후 6 05 26](https://user-images.githubusercontent.com/116433637/206447671-698954e0-f2b2-4950-ae50-0f297af9dd45.png)






![스크린샷 2022-12-08 오후 7 26 19](https://user-images.githubusercontent.com/116433637/206447711-71b5c6e4-bae0-4a49-81a7-0528b89ba2bb.png)







<학습 목표>
1. 회원가입, 로그인을 구현
2. 인증/인가를 이해하고 JWT를 활용하여 게시글을 처리
3. JPA 연관관계를 이해하고 회원과 게시글을 구현





<요구 사항>
1. 전체 게시글 목록 조회 API
    - 제목, 작성자명(username), 작성 내용, 작성 날짜를 조회하기
    - 작성 날짜 기준 내림차순으로 정렬하기
2. 게시글 작성 API
    - 토큰을 검사하여, 유효한 토큰일 경우에만 게시글 작성 가능
    - 제목, 작성자명(username), 작성 내용을 저장하고
    - 저장된 게시글을 Client 로 반환하기
3. 선택한 게시글 조회 API
    - 선택한 게시글의 제목, 작성자명(username), 작성 날짜, 작성 내용을 조회하기 
    (검색 기능이 아닙니다. 간단한 게시글 조회만 구현해주세요.)
4. 선택한 게시글 수정 API
    - ~~수정을 요청할 때 수정할 데이터와 비밀번호를 같이 보내서 서버에서 비밀번호 일치 여부를 확인 한 후~~
    - 토큰을 검사한 후, 유효한 토큰이면서 해당 사용자가 작성한 게시글만 수정 가능
    - 제목, 작성 내용을 수정하고 수정된 게시글을 Client 로 반환하기
5. 선택한 게시글 삭제 API  
    - ~~삭제를 요청할 때 비밀번호를 같이 보내서 서버에서 비밀번호 일치 여부를 확인 한 후~~
    - 토큰을 검사한 후, 유효한 토큰이면서 해당 사용자가 작성한 게시글만 삭제 가능
    - 선택한 게시글을 삭제하고 Client 로 성공했다는 메시지, 상태코드 반환하기
