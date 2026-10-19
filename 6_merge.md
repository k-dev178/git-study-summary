* 출처 : https://github.com/HwangNara/git-class/blob/master/beginner/README.md#branch-br
* 강의 : https://www.inflearn.com/course/git-for-work-part-1/dashboard?cid=324723

# merge

## fast-forward

현재 브랜치가 대상 브랜치의 조상일 때, 새 병합 커밋 없이 현재 브랜치 포인터를 대상 커밋으로 이동함.

![alt text](<6차시/6-1.png>)

![alt text](<6차시/6-2.png>)

## 3way merge

두 갈래로 나온 변경들을 합쳐서 새로운 커밋을 만듦

![alt text](<6차시/6-3.png>)

## squash

여러 커밋의 변경을 하나로 모아 stage함. `git merge --squash <브랜치>` 실행 후 `git commit`으로 커밋해야 함.

![alt text](<6차시/6-4.png>)
