* 출처 : https://github.com/HwangNara/git-class/blob/master/beginner/README.md#branch-br
* 강의 : https://www.inflearn.com/course/git-for-work-part-1/dashboard?cid=324723

# stash

* 작업 하던 내용을 임시 저장
* 브랜치에서 작업하다가 다른 브랜치로 변경해야 하는데 커밋은 하고 싶지 않은 경우 사용

```zsh
git stash # stash 함
git stash list # 임시 저장한 작업 목록 확인
git stash pop # 최근 작업을 적용하고, 성공하면 목록에서 제거
```

기본 stash는 추적 중인 파일의 변경을 저장함. 새 파일도 포함하려면 `git stash -u`를 사용함.

### 실습 결과

![alt text](<5차시/5-1.png>)
![alt text](<5차시/5-2.png>)

참고: [Git 공식 문서 — stash](https://git-scm.com/docs/git-stash)
