## 1. search-box css
search-box : 검색 기능 구현  
nav bar는 중앙에 유지하되 search box를 오른쪽에 둘 방법을 고민  
position:abosolute;로 하고 right:15px; 이렇게 하면 오른쪽에서 살짝 떨어져서 위치를 고정 가능

## 2. flex box 공부
https://d2.naver.com/helloworld/8540176

## 3. json-server
0.17.4 버전으로 설치해서 json 파일에 데이터를 설정  
리액트 앱 포트 번호가 3000이니까 겹치지 않도록 포트번호 지정  

## 4. 모바일 반응형 웹
기존 pc 웹 페이지에서 보이는 메뉴바를 모바일에서는 햄버거 메뉴로 변경하기  
https://velog.io/@yudidip/%EB%B0%98%EC%9D%91%ED%98%95-%ED%97%A4%EB%8D%94-%EB%A7%8C%EB%93%A4%EA%B8%B0React
처음 해보는 일이었는데 위의 링크를 통해서 적용

## 5. react bootstrap css 수정
https://think0wise.tistory.com/24
custom 할 방법을 도움 받음

## 6. redux, redux-thunk 사용
Navbar 클릭시 field별로 분류된 product만 보여줘야 하는데 오류로 인해 좀 헤맸다  
차분히 error 메세지를 확인하니 ProductAll.js에서 map 오류가 나서 문제인 것으로 보여  
```js
{productList?.map((menu) => (
```
?를 붙여 수정  
그래도 Navbar 클릭시 product가 안 나와서 console.log를 찍었는데 fieldProducts는 값이 잘 나오고 있었음  
해결방법은 ! reducer에서 payload 값을 넣을 때, fieldProducts로 넣어야 하는데 data로 넣고 있었다  
redux 사용법을 익히자  
