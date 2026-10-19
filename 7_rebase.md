* 출처 : https://github.com/HwangNara/git-class/blob/master/beginner/README.md#branch-br
* 강의 : https://www.inflearn.com/course/git-for-work-part-1/dashboard?cid=324723

# rebase

작업 브랜치의 커밋을 기준 브랜치 위에 다시 적용함.

```zsh
git switch <작업_브랜치>
git rebase <기준_브랜치>

# 충돌이 발생하면 파일을 수정한 뒤 해결한 파일을 stage
git add <해결한_파일>
git rebase --continue
```

![alt text](<7차시/7-1.png>)

![alt text](<7차시/7-2.png>)

참고: [Git 공식 문서 — rebase](https://git-scm.com/docs/git-rebase)
