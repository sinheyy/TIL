### useState
- useStates는 array를 반환
- 초기값이 담긴 state, state값을 변경해주는 함수 이 두 가지를 반환
-	변수는 re-render 될 때마다 초기화가 됨
-	State 값은 비동기적으로 처리됨

### function
그냥 : play("scissors")  
콜백 함수 형태 : () => play("scissors")  

- UI 부를 때(render 시), 함수를 실행하기 때문에 클릭을 안해도 print 되는 것을 확인할 수 있음  
-> 이럴 때는 콜백 함수 형태로 함수 전달하기  
-> 그냥 하면 처음 render 시에 함수가 실행되어버림  
★ 전달해줄 매개변수가 있는 경우에는 반드시 함수를 콜백 형태로 전달해주자


### Object.keys()
```JavaScript
let itemArray = Object.keys(choice);  // choice 객체를 배열화
```
Object.keys()
객체의 key 값만 뽑아서 array로 만들어줌

### $

```JavaScript
`box ${result}`
```

$ 사용 시 +의 역할
https://peamexx.tistory.com/197 참고

### display: flex
```js
.container{
    display: flex;
    justify-content: center;/*가로정렬*/
    align-items: center;/*세로정렬*/
}
```
- display: flex : 아이템들을 flexible하게 조절하기 좋음
- 같은 영역에 있는 아이템들을 세로가 아닌 가로 정렬로 바꿔버림
- flex-direction: column; 추가하면 원상복귀 가능


### 조건부 렌더링
```js
{/*<div>{weather && weather.name}</div>*/}
<div>{weather?.name}</div>
```
둘 다 같은 역할을 함


### 단방향 소통
부모가 모든 함수와 state를 가지고 있으면 자식에게 넘길 수 있음  
weather-app에서  
App이 WeatherInfo와 WeatherButton에게 필요한 정보를 모두 가지고 있고 필요한 정보는 자식들에게 넘겨줌  
자식들은 App이 준 걸로만 작업을 함 -> App이 나중에 그 정보를 받아다가 다른 데에도 넘겨줄 수 있게 됨  


### url 디자인 - restfult routes  
/subjects/:id  
':' 파라미터라는 뜻  
id는 가변적인 값  

### HTTP verbs
get : 데이터 가져올 때
post : 새로운 게시물을 생성할 때
put : 기존 데이터를 수정할 때
delete : 데이터 삭제

### navigate
```js
    const goProductPage = () => {
        navigate("/products?q=pants");  // query(pants인 값만 보여줘) 추가
    }
```
? 쿼리 뒤에 있는 값은 url 경로에 영향을 미치지 않음  


### redirect
예를 들어, 로그인 한 사람만 페이지를 접근하도록 하기 위해 계정 관련 페이지를 보호하고 미로그인일 때는 다른 페이지로 redirect 시킴  
Navigate 컴포넌트가 redirect를 도와줌(useNavigate랑 다름)  
