# nvm이란?
`node.js`의 버전관리를 위한 툴

# 설치된 node.js의 목록
```bash
$ nvm ls
```

# node.js 설치
```bash
$ nvm install 12.14.1
```

# 설치된 node.js 사용(관리자 권한 열기 필수)
```bash
$ nvm use 12.14.1
```

# 설치된 node.js의 버전 확인
```bash
$ node -v
```
# 설치된 node.js 삭제
```bash
$ nvm uninstall 12.21.0
```

# npm이란?
`npm(Node Package Manager)`은 전 세계의 개발자들이 만든 다양한 기능(패키지, 모듈)들을 관리

# npm 초기화
```bash
$ npm init -y //package.json 생성
```

# npm 패키지 설치(parcel-bundler)
## 개발 서버 열기 등 기능을 포함한 라이브러리
```bash
$ npm install -D parcel-bundler
```

# npm 패키지 설치(lodash)
```bash
$ npm install lodash
```

# "devDependencies"과 "dependencies"의 차이
dependencies : 플래그가 없으면 일반 의존성 설치 (웹 브라우져에서 동작 필요할 수 있음)  

devDependencies : '-D' 플래그가 있으면 개발용 의존성 패키지 설치 (개발할때만 필요, 개발을 할때 도움을 주는 개발 라이브러리)  
`npm install -D(npm install --save-dev)`로 설치 했을때 외부 라이브러리가 이 안에 종속된다.


# package.json의 scripts부분에 parcel-bundler 명령어 추가
```plaintext
"scripts": {  
  "dev" : "parcel index.html",  
  "build" : "parcel build index.html"  
}  
```

# parcel 개발 서버 실행
```bash
$ num run dev;  
$ num run build;
```  
`dev` 와 `build`의 차이점  
`dev`는 개발 서버를 만들어 실행할 수 있도록 만들어줌  
`build`는 브라우저가 해석할 수 있도록하는 용도(개발용 x), 코드를 난독화 하여 만들어 줌

# .gitignore 역할
 `git저장소`에 저장하지 않을 파일들을 명시하여 push명령을 실행 시 명시된 파일을 제외한 파일들을 `Repository`에 저장한다.

