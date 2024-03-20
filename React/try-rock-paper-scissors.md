# Rock-Paper-Scissors
## 1.
<b>상황</b>  
처음에 count 함수 호출 시 인수로 result를 넣었는데 점수가 바로 화면에 나타나지 않음  
Console.log로 값을 출력해봄  
result 값이 처음에 없어 문제가 발생한 것을 확인  
<br/>
<b>해결 방법</b>  
처음 시작할 때 result에는 null이 들어있기 때문에 하나씩 밀림
-> count 인수로 똑같이 judgement로 승패 판단한 것을 넣어 해결
<br/><br/>
<b>관련 코드</b>
```JavaScript
  // user가 버튼을 클릭할 때,
  const play = (userChoice) => {
    console.log("선택됨 - ", userChoice);
    setUserSelect(choice[userChoice]);

    // computerChoice 랜덤하게 값 받아서 set
    let computerChoice = randomChoice();
    setComputerSelect(computerChoice);

    // 승패 판단
    setResult(judgement(choice[userChoice], computerChoice));

    count(judgement(choice[userChoice], computerChoice));

  }

  // 점수 계산
  const count = (result) => {
    // result에 따른 점수 계산
    if (result == "win") {
      setUserScore(userScore + 1);
    }
    else if (result == "lose") {
      setComScore(comScore + 1);
    }

    //console.log("result", result,"user:", userScore, "com:", comScore);
  }

```

