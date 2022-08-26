# React+TypeScript Cheatsheets 한국어판 🇰🇷

TypeScript에 입문하는 React 개발자를 위한 치트시트(Cheetsheets)

---

<a href="https://github.com/typescript-cheatsheets/react/issues/81">
  <img
    height="90"
    width="90"
    alt="react + ts logo"
    src="https://user-images.githubusercontent.com/6764957/53868378-2b51fc80-3fb3-11e9-9cee-0277efe8a927.png"
    align="left"
  />
</a>

[**웹 다큐먼트**](https://react-typescript-cheatsheet.netlify.app/docs/basic/setup) |
[**영어판**](https://github.com/typescript-cheatsheets/react-typescript-cheatsheet-es) |
[프로젝트에 기여하기]() |
[질문하기]()

:wave: 본 리포지토리는 [@ryan_kim_kr](https://twitter.com/ryan_kim_kr)에 의해 관리되고 있습니다. 개발자님이 React와 함께 TypeScript를 사용해보고자 하시다니 정말 기쁜 소식이군요! 잘못된 부분이 발견되어 수정이 필요하거나 누락된 부분이 있다면 개선 되어야 할 사항을 [이슈 등록](https://github.com/typescript-cheatsheets/react-typescript-cheatsheet-kr/issues/new)해 주시기 바랍니다. :+1:

---

[![All Contributors](https://img.shields.io/github/contributors/typescript-cheatsheets/react-typescript-cheatsheet?color=orange&style=flat-square)](/COLABORADORES.md)

# All React + TypeScript Cheatsheets

- [기초 치트시트(The Basic Cheatsheet)]()는 React 개발자가 React app에서 TS 사용을 시작하는 것에 도움을 주기 위한 내용이 주를 이룹니다.
  - 모범 사례(Best Practices)라고 여겨지는, 복사 + 붙여넣기 가능한 예시
  - 기본적인 TS Types 사용법과 설정 방법
  - 자주 묻는 질문(FAQ)에 대한 답변
  - Generic type logic은 깊이 다루지 않습니다. 그 대신, 초심자들을 위해 간단한 트러블슈팅 기술들을 소개합니다.
  - 기초 치트시트는 개발자가 TypeScript에 대해 너무 많은 공부를 하지 않고서도 **시간 효율적**으로 React 개발에 TypeScript를 빠르게 사용할 수 있도록 돕는 데 그 목적이 있습니다.
- [고급 치트시트(The Advanced Cheatsheet)]()는 재사용 가능한 type utilities/functions/render prop/higher order copmonents 또는 TS+React 라이브러리를 작성하고자 하는 개발자를 위해 generic types의 고급 사용법에 대한 이해를 돕습니다.
  - 전문적인 개발자들을 위한 다양한 팁과 요령들을 소개합니다.
  - DefinitelyTyped에 기여하기 위한 조언을 드립니다.
  - 고급 치트시트는 개발자가 TypeScript를 최대한 활용할 수 있도록 돕는 데 그 목적이 있습니다.
- [마이그레이팅 치트시트(The Migrating Cheatsheet)]()는 대규모 코드베이스를 JS 또는 Flow에서 TypsScript로 점진적으로 마이그레이션 하는 것에 대한 경험자의 조언을 얻는데 도움을 줍니다.
  - 우리는 여러분이 마이그레이션을 하도록 설득하려는 것이 아니며, 이미 그렇게 하고자 결정한 사람들을 돕고자 합니다.
  - ⚠️ 이 치트시트는 새롭게 만들어진 치트시트 입니다. 따라서 도움을 주고자 하는 모든 분들을 환영합니다.
- [HOC 치트시트(The HOC Cheatsheet)]()는 예시와 함께 HOC를 작성하는 방법을 알려줍니다.
  - [Generics](https://www.typescriptlang.org/docs/handbook/2/generics.html)에 대한 이해가 선행되어야 합니다.
  - ⚠️ 이 치트시트는 새롭게 만들어진 치트시트 입니다. 따라서 도움을 주고자 하는 모든 분들을 환영합니다.

---

## 기초 치트시트 (Basic Cheatsheet)

### 기초 치트시트 목차

<details>

<summary><b>목차 확장하기</b></summary>

- [섹션 1: React에 TypeScript 설정하기]()
    <!--START_SECTION:setup-toc-->
  - [전제조건]()

</details>

<!--START-SECTION:setup-->

### 섹션 1: React에 TypeScript 설정하기

#### 시작하기 전 필요한 사항

1. [React](https://reactjs.org)에 대한 충분한 이해
2. [TypeScript Types](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html) ([2ality's guide](http://2ality.com/2018/04/type-notation-typescript.html)를 알고있으면 문서를 이해하는데 도움이 됩니다. 만약 TypeScript를 처음 접하는 분이라면,[chibicode’s tutorial](https://ts.chibicode.com/todo/).)를 참고해 보세요.
3. [the TypeScript section in the official React docs](https://reactjs.org/docs/static-type-checking.html#typescript) 읽기
4. [the React section of the new TypeScript playground](http://www.typescriptlang.org/play/index.html?jsx=2&esModuleInterop=true&e=181#example/typescript-with-react) 읽기 (선택사항: [the playground's](http://www.typescriptlang.org/play/index.html) Example Section의 40+ examples 단계를 수행해 보기)

이 가이드는 독자가 가장 최신 버전의 TypeScript와 React를 사용한다고 가정합니다. 이전 버전에 대한 사항은 확장 가능한 `<details>` 태그로 확인 가능합니다.

#### VS Code 확장 프로그램(Extensions)

- 리펙토링 보조 https://marketplace.visualstudio.com/items?itemName=paulshen.paul-typescript-toolkit
- R+TS Code Snippets (여러가지 확장 프로그램이 있습니다...)
  - https://marketplace.visualstudio.com/items?itemName=infeng.vscode-react-typescript
  - https://www.digitalocean.com/community/tutorials/the-best-react-extension-for-vs-code
- TypeScript 공식 확장프로그램 https://code.visualstudio.com/docs/languages/typescript

#### React + TypeScript 입문자 키트

Cloud setups:

- [TypeScript Playground with React](https://www.typescriptlang.org/play?#code/JYWwDg9gTgLgBAKjgQwM5wEoFNkGN4BmUEIcA5FDvmQNwCwAUKJLHAN5wCuqWAyjMhhYANFx4BRAgSz44AXzhES5Snhi1GjLAA8W8XBAB2qeAGEInQ0KjjtycABsscALxwAFAEpXAPnaM4OANjeABtA0sYUR4Yc0iAXVcxPgEhdwAGT3oGAOTJaXx3L19-BkDAgBMIXE4QLCsAOhhgGCckgAMATQsgh2BcAGssCrgAEjYIqwVmutR27MC5LM0yuEoYTihDD1zAgB4K4AA3H13yvbAfbs5e-qGRiYspuBmsVD2Aekuz-YAjThgMCMcCMpj6gxcbGKLj8MTiVnck3gAGo4ABGTxyU6rcrlMF3OB1H5wT7-QFGbG4z6HE65ZYMOSMIA)는 코드를 실행하지 않고 Types를 디버깅만 하는 경우 사용할 수 있습니다.
- [CodeSandbox](http://ts.react.new) - cloud IDE, 매우 빠른 부팅 속도를 가집니다.
- [Stackblitz](https://stackblitz.com/edit/react-typescript-base) - cloud IDE, 매우 빠른 부팅 속도를 가집니다.

Local dev setups:

- [Next.js](https://nextjs.org/docs/basic-features/typescript): `npx create-next-app -e with-typescript` 명령어는 새로운 NextJS 프로젝트를 현재 폴더에 생성합니다.
- [Create React App](https://facebook.github.io/create-react-app/docs/adding-typescript): `npx create-react-app name-of-app --template typescript` 명령어는 새로운 NextJS 프로젝트를 새로운 폴더에 생성합니다.
- [Vite](https://vitejs.dev/): `npm create vite@latest my-react-ts-app -- --template react-ts`
- [Meteor](https://guide.meteor.com/build-tool.html#typescript): `meteor create --typescript name-of-my-new-typescript-app`
- [Ignite](https://github.com/infinitered/ignite#use-ignite-andross-infinite-red-andross-boilerplate) for React Native: `ignite new myapp`
- [TSDX](https://tsdx.io/): `npx tsdx create mylib` 명령어는 React+TS _라이브러리_ 를 생성합니다. (in future: [TurboRepo](https://twitter.com/jaredpalmer/status/1346217789942591488))

<details>
<summary><b>다른 도구들</b></summary>

아직 보완이 필요하지만 확인해 볼 만한 가치가 있는 도구들:

- [Snowpack](<https://www.snowpack.dev/#create-snowpack-app-(csa)>): `npx create-snowpack-app my-app --template app-template-react-typescript`
- [Docusaurus v2](https://v2.docusaurus.io/docs/installation) with [TypeScript Support](https://v2.docusaurus.io/docs/typescript-support)
- [Parcel](https://v2.parceljs.org/languages/typescript/)
- [JP Morgan's `modular`](https://github.com/jpmorganchase/modular): CRA + TS + Yarn Workspaces toolkit. `yarn create modular-react-app <project-name>`

Manual setup:

- [Basarat's guide](https://github.com/basarat/typescript-react/tree/master/01%20bootstrap)는 React + TypeScript + Webpack + Babel 을 **수동으로 설정** 할 경우 사용할 수 있습니다.
- 특히, `@types/react`와 `@types/react-dom`가 설치되어 있는지 확인이 필요합니다. ([익숙하지 않은 내용이라면 DefinitelyTyped project 에 대해 더 알아보세요.](https://definitelytyped.org/))
- 또한 많은 React + TypeScript bolierplates들이 있습니다. [우리의 다른 리소스 리스트](https://react-typescript-cheatsheet.netlify.app/docs/basic/recommended/resources/)를 확인해주세요.

</details>

#### 비디오 튜토리얼

아래의 7부로 구성된 "React Typescript Course" 비디오 시리즈를 통해 TypeScript with React에 대한 소개를 들을 수 있습니다.

<a href="https://www.youtube.com/watch?v=PL1NUl7fQ2I&list=PLG-Mk4wQm9_LyKE5EwoZz2_GGXR-zJ5Ml">
    <img
        width="200px"
        alt="react typescript course video series"
        src="https://i.imgur.com/IIG0Xu9.jpeg"
    />
</a>

<!--END-SECTION:setup-->
