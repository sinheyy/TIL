## 1. API 호출 오류
<b>상황</b>  
이메일도 다 verify 하고 5시간 정도 지났는데도 invalid key라고 에러가 남   
<br/>
<b>해결 방법</b>  
url을 잘못 쓴 거 였다...!  
벡틱을 사용해서 잘 해결함..
<br/><br/>
<b>관련 코드</b>

![image](https://github.com/sinheyy/TIL/assets/163747140/64f39599-5d78-45c1-8970-ee8daa7a2252)


## 2. npm react-spinners 내가 겪은 오류
<b>상황</b>  
- react-spinners 설치를 위해 "npm install --save react-spinners" 입력
-  아래와 같이 취약점이 뜨면서 스피너가 화면에 안 나옴  
-  audit fix도 해봤으나 잘 모르겠고 구글링 했는데 node.js 버전 문제인가 싶어서
-  16 버전도 설치해보고 했으나 해결이 안 됨  
<br/>
<b>해결 방법</b>  <br>
- 슬랙에 누가 질문한 걸 보고 npm start 하면 된다길래 시도해봤으나 안 됨  <br>
- 마지막으로 혹시나 해서 새로 create-react-app 해서 프로젝트를 만들고 js 파일 내용만 복붙<br>
- 다시 설치하고 그대로 다시 npm start했더니 spinner가 나옴!  <br>
<br/><br/>
<b>관련 코드</b>

![a](https://github.com/sinheyy/TIL/assets/163747140/a4127ed7-0603-48c5-b97e-0b09aac0383b)
![b](https://github.com/sinheyy/TIL/assets/163747140/d8dfaa40-f4ee-46ba-833f-05aef8379275)
![c](https://github.com/sinheyy/TIL/assets/163747140/44c01dc3-f5b9-4893-90d0-030b07f4da0d)


## 3. .env 사용해서 api key 숨기기
https://velog.io/@rmaomina/react-env
<br>
[https://shape-coding.tistory.com/entry/React-리액트에서-env-환경변수-사용하기](https://shape-coding.tistory.com/entry/React-%EB%A6%AC%EC%95%A1%ED%8A%B8%EC%97%90%EC%84%9C-env-%ED%99%98%EA%B2%BD%EB%B3%80%EC%88%98-%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0)
<br>
[https://velog.io/@sweetpumpkin/React-환경변수가-undefined로-나올-때](https://velog.io/@sweetpumpkin/React-%ED%99%98%EA%B2%BD%EB%B3%80%EC%88%98%EA%B0%80-undefined%EB%A1%9C-%EB%82%98%EC%98%AC-%EB%95%8C)
<br>
.env 파일을 root 폴더에 생성해서 REACT_APP을 붙여 api key를 적어두기  
gitignore에 .env 추가하기  
repo 다시 생성하느라 열심히 심은 잔디가 2개나 날아가버린 사태 발생했지만... 앞으로 다시 열심히 하겠습니다 ㅠ


## 4. 도시명으로 날씨 검색할 때 에러 처리 방식
https://week-book.tistory.com/entry/React-fetch-사용법-LoadingErrorGETPOST
<br>
try, catch 사용하기, if(response!=ok) -> 도시 이름 제대로 입력해달라고 alert
