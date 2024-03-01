# Git
- 파일 버전 기록해주는 프로그램
- git이 파일 저장해두는 장소: repository
- 온라인 repository의 장점
  - 컴퓨터가 고장나도 복구 가능
  - 협업 가능
<br><br>

# Git 명령어 정리 

repository 생성하기 (해당 작업폴더에서 git을 사용하겠다.)
```
git init
```

기본 브랜치 이름을 main으로 설정하기
```
git branch -M main
```

버전을 기록할 파일들을 staging area로 옮기기
```
git add .
```

고른 파일의 버전을 repository에 기록하기
```
git commit -m '커밋 메시지'
```

로컬저장소를 원격저장소로 올리기
- git push할 때 -u 추가하면 주소 기억하라는 뜻이다.
```
git push -u 원격저장소주소 로컬브랜치명
```

git에서 변수 문법 사용하기
```
git remote add 변수명 원격저장소주소
```

이 오류는 로컬 저장소의 브랜치가 원격 저장소의 브랜치보다 이전 커밋을 가리키고 있어서 발생합니다. 이를 해결하기 위해서는 먼저 로컬 브랜치를 원격 브랜치에 통합해야 합니다.
또는 먼저 로컬 저장소의 변경 사항을 가져와서 로컬 브랜치를 업데이트하고, 그 다음에 다시 푸시합니다.
```
git pull https://github.com/wvssm/TIL.git main
git push https://github.com/wvssm/TIL.git main
```