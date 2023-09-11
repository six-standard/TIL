# TypeScript
> 타입스크립트는 **자바스크립트의 슈퍼셋**인 오픈소스 프로그래밍 언어이다.  
> **마이크로소프트**에서 개발, 유지하고 있으며 엄격한 문법을 지원한다.   
> **클라이언트 사이드와 서버 사이드**를 위한 개발에 사용할 수 있다.  
> 타입스크립트에서 자신이 원하는 **타입을 정의하고 프로그래밍을 하면,  
> 자바스크립트로 컴파일**되어 실행할 수 있다.  
> **- 위키 백과 -**


타입스크립트는 **'자바스크트의 단점들을 전부 보완해 만든 확장 버전'** 이라고 할 수 있다.
변수나 함수에 타입을 부여하고, 오류 검출을 돕는 등의 기능을 한다.

## 사용하는 이유?
- **오류 검출이 편하다.**  
타입스크립트는 파일에 타입을 부여한다.  
그로 인해 코드 작성시 알맞지 않은 타입이나 값을 넣거나, 타입이 아얘 없을 경우 오류가 출력된다.  

- **실행 속도가 빠르다.**  
자바스크립트는 동적 타입의 인터프리터 언어다.  
이로 인해 타입을 실행시 결정하여 적용하는데, 컴퓨터에게 오류 검증을 맡기는 꼴이니 실행 속도가 느리다.  
하지만 타입스크립트는 사람이 오류 체크와 타입 선택을 하기 떄문에 컴퓨터의 일을 덜 수 있다. 덕분에 속도가 빠르다.  

- **안정적이다.**  
자바스크립트는 타입 명시가 없어, 유지보수중 변수의 타입 짐작이 어렵다.  
또한 자바스크립트는 컴파일시 오류를 검출하지 않아, 운영중 오류가 발생할 수도 있다.  
하지만 타입스크립트는 타입 명시와 컴파일 과정에서의 오류 검출로 인해 더 안정적이고, 유지보수시에 좋다.  

## 개발환경 세팅 방법
참고로 해당 방식은 **리액트 기반**이다.  
그러므로, 만약 Next.js나 Vue.js와 같은 프레임워크를 사용한다면 다른 방법을 찾아봐야 한다.

 - ### 설치
    프로젝트의 경로로 이동 후 해당 명령어를 사용한다.
    ```
    npm install typescript (npm의 경우)
    yan add typescript (yarn의 경우)
    ```
    그 후 프로젝트 폴더 내부에서 `tsc —init` 명령어를 사용하면 **tsconfig.json 파일**이 생성된다

 - ### 설정 수정
    ```jsx
    {
      "compilerOptions": {
        "target": "es5",
        "module": "commonjs",
        "strict": true,
        "esModuleInterop": true,
        "outDir": "./dist"
      } 
    }
    ```
    
    - **target**: 컴파일된 코드가 어떤 환경에서 실행될 지 정의한다.
    - **module**: 컴파일된 코드가 어던 모듈 시스템을 사용할지 정의한다.
    - **strict**: 모든 타입 체킹 옵션을 활성화할지 말지 정의한다.
    - **esModuleInterop**: commonjs 모듈 형태로 이루어진 파일을 es2015 모듈 형태로 불러올 수 있게 해준다.
    - **outDir**: 컴파일 후 생성될 js 파일들의 위치를 지정한다.

    자세한 내용은 <b><a href="http://json.schemastore.org/tsconfig">해당 페이지</a></b>에서 확인할 수 있다.