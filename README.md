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
2. [TypeScript Types](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html)주제에 대한 이해 ([2ality's guide](http://2ality.com/2018/04/type-notation-typescript.html)를 알고있으면 문서를 이해하는데 도움이 됩니다. 만약 TypeScript를 처음 접하는 분이라면,[chibicode’s tutorial](https://ts.chibicode.com/todo/)를 참고해 보세요.)
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

### Section 2: 시작하기

<!--START-SECTION:function-components-->

#### 함수 컴포넌트

함수 컴포넌트는 `props`를 매개변수로 받고 JSX element를 반환하는 일반적인 함수로 작성될 수 있습니다.

```tsx
// props의 타입 정의 - 더 많은 예시는 "컴포넌트 Props 타이핑"에서 확인할 수 있습니다.
type AppProps = {
  message: string;
}; /* export 한다면 consumer가 extend할 수 있도록 `interface`를 사용하세요. */

// 함수 컴포넌트를 정의할 수 있는 가장 쉬운 방법; return type은 추론됩니다.
const App = ({ message }: AppProps) => <div>{message}</div>;

// 실수로 다른 타입을 반환하였을 때 에러가 raise 되도록 return type을 명시할 수 있습니다.
const App = ({ message }: AppProps): JSX.Element => <div>{message}</div>;

// type 선언을 함수 컴포넌트 선언에 포함시킬 수 있습니다.;이 방법은 prop types에 이름을 붙이지 않아도 되지만 코드가 반복됩니다.
const App = ({ message }: { message: string }) => <div>{message}</div>;
```

> Tip: type destructure 선언을 위해 [Paul Shen's VS Code Extension](https://marketplace.visualstudio.com/items?itemName=paulshen.paul-typescript-toolkit)를 사용할 수도 있습니다. ([keyboard shortcut](https://twitter.com/_paulshen/status/1392915279466745857?s=20)을 추가 하세요.)

<details>

<summary><b><code>React.FC</code>가 권장되지 않는 이유는 무엇일까요? <code>React.FunctionComponent</code>/<code>React.VoidFunctionComponent</code>는 어떤가요?</b></summary>

React+TypeScript codebases에서 다음 보았을 수 있습니다.

```tsx
const App: React.FunctionComponent<{ message: string }> = ({ message }) => <div>{message}</div>;
```

하지만, 현재 `React.FunctionComponent` (또는 간략하게 써서 `React.FC`)는 [권장되지 않는다는 것](https://github.com/facebook/create-react-app/pull/8177)에 대부분의 사람들이 동의합니다. 물론 이 주제에 대한 미묘한 의견 차이가 있을 수는 있지만, 만약 이 의견에 동의하고 `React.FC`를 당신의 코드베이스에서 제거하고 싶다면, [이 jscodeshift codemond](https://github.com/gndelia/codemod-replace-react-fc-typescript)를 사용할 수 있습니다.

"일반적인 함수" 버전과의 차이점들은 다음과 같습니다.

- `React.FunctionComponent`는 return type을 명시적으로 밝힙니다. 하지만 일반적인 함수 버전은 암시적입니다(또는 추가적인 어노테이션(annotation)이 필요합니다).

- `displayName`, `propTypes`, 그리고 `defaultProps`와 같은 static properties를 위한 자동완성(autocomplete)과 타입 체크(Typechecking)를 지원합니다.

  - `React.FunctionComponent`와 함께 `defaultProps`을 사용하는데 몇 가지 알려진 문제가 있습니다. [문제에 대한 자세한 내용](https://github.com/typescript-cheatsheets/react/issues/87)을 확인하세요. 우리는 개발자님이 찾아볼 수 있는 별개의 `defaultProps` 섹션을 제공하고 있습니다.

- [React 18 type 업데이트](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/56210) 이전에는, `React.FunctionComponent`이 `children`에 대한 암시적인 정의(implicit definition)를 제공했었습니다. 이것은 열띤 토론 과정을 거쳤고 결과적으로 [`React.FC`가 Create React App TypeScript template에서 제거](https://github.com/facebook/create-react-app/pull/8177)된 이유 중 하나가 되었습니다.

```tsx
// React 18 types 이전
const Title: React.FunctionComponent<{ title: string }> = ({ children, title }) => (
  <div title={title}>{children}</div>
);
```

<details>
<summary>(Deprecated)<b><code>React.VoidFunctionComponent</code> 또는 <code>React.VFC</code> 사용하기</b></summary>

[@types/react 16.9.48](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/46643)에서, `React.VoidFunctionComponent` 또는 `React.VFC` type은 `children`을 명시적으로 타이핑(typing) 하기 위해 추가되었습니다.
하지만, `React.VFC`와 `React.VoidFunctionComponent`는 React 18 (https://github.com/DefinitelyTyped/DefinitelyTyped/pull/59882) 에서 더이상 사용되지 않게 되었습니다(deprecated). 따라서 이 임시방편은 React 18+ 에서 더이상 권장되지 않습니다.

일반적인 함수 컴포넌트나 `React.FC`를 사용해 주세요.

```ts
type Props = { foo: string };

// 지금은 괜찮지만, 미래에는 에러를 발생시킬 것입니다.
const FunctionComponent: React.FunctionComponent<Props> = ({ foo, children }: Props) => {
  return (
    <div>
      {foo} {children}
    </div>
  ); // OK
};

// 지금은 에러를 발생시키고, 미래에는 더이상 사용되지 않을것입니다.(Deprecated)
const VoidFunctionComponent: React.VoidFunctionComponent<Props> = ({ foo, children }) => {
  return (
    <div>
      {foo}
      {children}
    </div>
  );
};
```

</details>

- _미래에는_, props를 자동으로 `readonly` 라고 표시할 수도 있습니다. 하지만, props 객체가 파라미터 리스트에서 destructure 된다면, 이것은 의미없는 행동 입니다.

대부분의 경우에는 어떤 syntax를 사용하던지 큰 차이가 없지만, `React.FunctionComponent`의 보다 명시적인 특성을 선호하는 것이 좋을것입니다.

</details>

<details>
<summary><b>주의해야 할 사항</b></summary>

다음의 패턴은 지원되지 않습니다. :

**조건부 렌더링(conditional rendering)**

```tsx
const MyConditionalComponent = ({ shouldRender = false }) => (shouldRender ? <div /> : false); // JS 에서도 이렇게 하지 마십시오.
const el = <MyConditionalComponent />; // 에러를 throw 합니다.
```

이 패턴이 지원되지 않는 이유는 컴파일러의 한계 때문입니다. 함수 컴포넌트는 JSX expression 또는 `null` 이외의 다른 어떤 것도 반환할 수 없습니다. 반환할 수 없는 것이 반환된다면 해당 타입은 `Element`에 할당될 수 없다는 에러 메세지를 보게될 것입니다. ("{the other type} is not assignable to `Element`.")

**Array.fill**

```tsx
const MyArrayComponent = () => Array(5).fill(<div />);
const el2 = <MyArrayComponent />; // throws an error
```

아쉽게도 함수의 타입을 annotate 하는 것은 아무런 도움이 되지 않을것입니다. React가 지원하는 다른 특별한 타입(exotic type)을 반환하고자 한다면 타입 표명(type assertion)을 수행해야 합니다. :

```tsx
const MyArrayComponent = () => Array(5).fill(<div />) as any as JSX.Element;
```

[여기서 @ferdaber 의 설명을 확인해보세요](https://github.com/typescript-cheatsheets/react/issues/57).

</details>

<!--END-SECTION:function-components-->

<!--START-SECTION:hooks-->

#### Hooks

Hook은 [`@types/react` v16.8 이상부터 지원됩니다](https://github.com/DefinitelyTyped/DefinitelyTyped/blob/a05cc538a42243c632f054e42eab483ebf1560ab/types/react/index.d.ts#L800-L1031).

#### useState

타입 추론(Type inference)은 간단한 값들에 잘 작동합니다:

```tsx
const [state, setState] = useState(false);
// `state` 는 boolean 으로 추론됩니다.
// `setState` 는 boolean 값 만을 받습니다.
```

타입 추론에 복잡한 타입을 사용해야 한다면 [추론된 타입(Inferred Types) 사용하기](https://react-typescript-cheatsheet.netlify.app/docs/basic/troubleshooting/types/#using-inferred-types) 도 확인해보세요.

하지만 많은 hook 들은 null 같은 값를 디폴트 값으로 초기화 하기 때문에 어떻게 타입을 지정하는지 궁금할 수 있습니다. 명시적으로 타입을 선언하고, union type을 사용하세요.:

```tsx
const [user, setUser] = useState<User | null>(null);

// later...
setUser(newUser);
```

만약 useState설정 직후에 state가 초기화되고 그 이후에 항상 값을 가진다면, 타입 표명(type assertions)을 사용할 수도 있습니다.

```tsx
const [user, setUser] = useState<User>({} as User);

// later...
setUser(newUser);
```

이 방법은 일시적으로 타입스크립트 컴파일러에게 `{}`가 `User`의 type이라고 "거짓말" 합니다. 그 후에 `user` state를 설정하여야 합니다. 그렇지 않으면 나머지 코드가 `user`는 `User` 타입이라는 사실에 의존고 이것은 런타입 에러로 이어질 수 있습니다.

#### useReducer

Reducer actions를 위해 [Discriminated Unions](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes-func.html#discriminated-unions)를 사용할 수 있습니다. reducer의 return type을 정의하는 것을 잊지 마세요. 그렇지 않으면 타입스크립트가 return type을 추론할 것입니다.

```tsx
import { useReducer } from "react";

const initialState = { count: 0 };

type ACTIONTYPE = { type: "increment"; payload: number } | { type: "decrement"; payload: string };

function reducer(state: typeof initialState, action: ACTIONTYPE) {
  switch (action.type) {
    case "increment":
      return { count: state.count + action.payload };
    case "decrement":
      return { count: state.count - Number(action.payload) };
    default:
      throw new Error();
  }
}

function Counter() {
  const [state, dispatch] = useReducer(reducer, initialState);
  return (
    <>
      Count: {state.count}
      <button onClick={() => dispatch({ type: "decrement", payload: "5" })}>-</button>
      <button onClick={() => dispatch({ type: "increment", payload: 5 })}>+</button>
    </>
  );
}
```

[TypeScript Playground에서 보기](https://www.typescriptlang.org/play?#code/LAKFEsFsAcHsCcAuACAVMghgZ2QJQKYYDGKAZvLJMgOTyEnUDcooRsAdliuO+IuBgA2AZUQZE+ZAF5kAbzYBXdogBcyAAwBfZmBCIAntEkBBAMIAVAJIB5AHLmAmgAUAotOShkyAD5zkBozVqHiI6SHxlagAaZGgMfUFYDAATNXYFSAAjfHhNDxAvX1l-Q3wg5PxQ-HDImLiEpNTkLngeAHM8ll1SJRJwDmQ6ZIUiHIAKLnEykqNYUmQePgERMQkY4n4ONTMrO0dXAEo5T2aAdz4iAAtkMY3+9gA6APwj2ROvImxJYPYqmsRqCp3l5BvhEAp4Ow5IplGpJhIHjCUABqTB9DgPeqJFLaYGfLDfCp-CIAoEFEFeOjgyHQ2BKVTNVb4RF05TIAC0yFsGWy8Fu6MeWMaB1x5K8FVIGAUglUwK8iEuFFOyHY+GVLngFD5Bx0Xk0oH13V6myhplZEm1x3JbE4KAA2vD8DFkuAsHFEFcALruAgbB4KAkEYajPlDEY5GKLfhCURTHUnKkQqFjYEAHgAfHLkGb6WpZI6WfTDRSvKnMgpEIgBhxTIJwEQANZSWRjI5SdPIF1u8RXMayZ7lSphEnRWLxbFNagAVmomhF6fZqYA9OXKxxM2KQWWK1WoTW643m63pB2u+7e-3SkEQsPamOGik1FO55p08jl6vdxuKcvv8h4yAmhAA)

<details>

<summary><b><code>Redux</code>에서 <code>Reducer</code>와 함께 사용하기</b></summary>

Reducer funciton을 작성하기 위해 [redux](https://github.com/reduxjs/redux)를 사용하는 경우, return type을 처리하는 `Reducer<State, Action>` 형식의 편리한 helper를 사용할 수 있습니다.

위의 reducer example은 다음과 같이 바뀔 수 있습니다. :

```tsx
import { Reducer } from 'redux';

export function reducer: Reducer<AppState, Action>() {}
```

</details>
