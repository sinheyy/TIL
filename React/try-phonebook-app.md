## reducer 폴더에 대해
reducer 폴더를 따로 만들어주는 이유는 앞으로 기능에 따라 reducer가 여러 개 생길 수 있어서이다.  

## payload 간단히 적기
```js
dispatch({ type: "ADD_CONTACT", payload: { name: name, phoneNumber: phoneNumber } });
```

```js
dispatch({ type: "ADD_CONTACT", payload: { name, phoneNumber } });
```

payload에서 이름이 같으면 이렇게 줄여서 쓸 수 있다.(ES6 JS 문법)

## destructure
```js
const {type, payload} = action
```
action을 이렇게 distructure 해주면 일일이 action.을 안 붙여도 된다!

## redux에서 state 들고 오는게 더 복잡할 때는 그냥 props 쓰기
부모->자식 간은 props 편하게 쓸 수 있다~
