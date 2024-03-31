## payload integer
https://velog.io/@boyfromthewell/React-Redux-4-more-dispatch  
payload로 step 값을 reducer로 전달했는데  
3+2=5가 되어야 하는데 32로 나옴  
console에 찍었을 때 step이 string으로 전달되고 있는 것 같았음  
Number()를 씌워서 step을 전달했더니 해결
![image](https://github.com/sinheyy/TIL/assets/163747140/ddd333f9-e2c4-4726-ba04-ba46057cc8d8)
