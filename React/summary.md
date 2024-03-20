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
