* 출처 : https://github.com/HwangNara/git-class/blob/master/beginner/README.md#branch-br
* 강의 : https://www.inflearn.com/course/git-for-work-part-1/dashboard?cid=324723

# reset

현재 브랜치를 직전 커밋으로 이동:

```zsh
git reset @~
# @는 HEAD, @~는 HEAD~1과 같음 (첫 번째 부모 커밋)
```

![alt text](<8차시/8-1.png>)

## --soft

* 현재 브랜치를 대상 커밋으로 이동하고, index와 작업 파일은 유지함.
* 깨끗한 상태에서 직전 커밋을 되돌리면, 그 커밋의 변경 내용이 Staged 상태로 남음.

![alt text](<8차시/8-2.png>)

## --mixed (기본)

* 현재 브랜치와 index를 대상 커밋으로 되돌리고, 작업 파일은 유지함.
* 변경 내용은 stage되지 않은 상태로 남으며, 대상 커밋에 없는 파일은 Untracked가 될 수 있음.

![alt text](<8차시/8-3.png>)

## --hard

* 현재 브랜치, index, 추적 중인 작업 파일을 대상 커밋에 맞춤.
* 커밋하지 않은 변경은 사라질 수 있으며 Git만으로 복구가 어려움. 이미 커밋한 내용은 reflog에 남아 있다면 복구할 수 있음.

![alt text](<8차시/8-4.png>)

참고: [Git 공식 문서 — reset](https://git-scm.com/docs/git-reset)
