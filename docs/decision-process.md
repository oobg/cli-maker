# 일자별 결정과정.

## 26.04.02
1. 프로젝트 신규 생성.
2. 패키지 매니저
    - 전통적인 `npm`? 아니면 엔스로픽에서 인수한 `bun`?
    - 학습 목적도 있으니 `bun` 으로 진행하자.
    - `bun` 설치 필요
2. 프로젝트 초기화
    - package.json 생성해야한다.
    - `bun init .` 로 생성.
    - README.md 에 AI 는 사용하지 않겠다고 작성했으니, 같이 생성된 `CLAUDE.md` 는 지워버리자
3. eslint 로 에러를 사전 검출하자.
    - eslint 공식 사이트의 빠른 시작을 따라가자.
    - `bun create @eslint/config@latest`
```
✔ What do you want to lint? · javascript
✔ How would you like to use ESLint? · problems
✔ What type of modules does your project use? · esm
✔ Which framework does your project use? · none
✔ Does your project use TypeScript? · No / Yes
✔ Where does your code run? · node
✔ Which language do you want your configuration file be written in? · ts
ℹ Jiti is required for Node.js <24.3.0 to read TypeScript configuration files.
✔ Would you like to add Jiti as a devDependency? · No / Yes
ℹ The config that you've selected requires the following dependencies:

eslint, @eslint/js, globals, typescript-eslint, jiti
✔ Would you like to install them now? · No / Yes
✔ Which package manager do you want to use? · bun
```
4. prettier 로 코드 포매팅하자.
    - prettier.io 공식 사이트의 빠른 시작을 따라가자.
    - `bun add --dev --exact prettier`
    - ignore 하고 rc 설정값은 이전 프로젝트 값을 가져왔다.
5. 소스 파일을 생성하자.
    - `src/main.ts` 를 진입점으로 가져가자.
