# 내가 겪은 GIT 에러들 정리

## 1
<b>발생 상황</b>  
![image](https://github.com/sinheyy/TIL/assets/163747140/d1ca1fe2-eb64-4a7d-bfd9-ec9dea06af3b)  
  
<b>해결 방법</b>  
https://velog.io/@booyouhada/git-error-src-refspec-main-does-not-match-any  
링크 참고하여 해결  
master가 branch default로 되어 있어서 문제 발생 -> git branch로 branch 확인하고 main으로 변경해줌  

## 2
<b>발생 상황</b>  
![image](https://github.com/sinheyy/TIL/assets/163747140/e93a6a32-8e77-4ddc-b3b0-01ebe8223357)  

<b>해결 방법</b>  
https://velog.io/@jytrack/Git-Error-failed-to-push-some-refs-to-...-%ED%95%B4%EA%B2%B0%ED%95%98%EA%B8%B0 참고  
pull 하고 push 하기

## 3
<b>발생 상황</b>  
![image](https://github.com/sinheyy/TIL/assets/163747140/93ef2569-81d4-43a5-a5cb-6ae9479dbd2a)  
Pull 하고 기다리는데 insert가 뜨는데 입력하려고 해도 키보드가 안 쳐짐

<b>해결 방법</b>  
https://velog.io/@ssmin0606/%EA%B0%9C%EB%B0%9C%ED%88%B4-Please-enter-a-commit-message-to-explain-why-this-merge-is-necessary-especially-if-it-merges-an-updated-upstream-into-a-topic-branch-%ED%95%B4%EA%B2%B0%ED%95%98%EA%B8%B0-git-bash 참고  
Esc 누르고 :wq 치고 엔터

## 4
<b>발생 상황</b>  
![image](https://github.com/sinheyy/TIL/assets/163747140/4ef467e6-8944-4c31-9193-56a582a49c6f)

git checkout 시 에러 발생

<b>해결 방법</b>  
[https://velog.io/@ssmin0606/%EA%B0%9C%EB%B0%9C%ED%88%B4-Please-enter-a-commit-message-to-explain-why-this-merge-is-necessary-especially-if-it-merges-an-updated-upstream-into-a-topic-branch-%ED%95%B4%EA%B2%B0%ED%95%98%EA%B8%B0-git-bash](https://kgw7401.tistory.com/65) 참고  
git stash

git checkout sinhey

git stash pop
