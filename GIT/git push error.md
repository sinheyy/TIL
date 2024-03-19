<b>발생 상황</b>  
$ git push origin main  
error: src refspec main does not match any  
error: failed to push some refs to 'https://github.com/~.git'  
  
<b>해결 방법</b>  
https://velog.io/@booyouhada/git-error-src-refspec-main-does-not-match-any  
링크 참고하여 해결  
master가 branch default로 되어 있어서 문제 발생 -> git branch로 branch 확인하고 main으로 변경해줌  
