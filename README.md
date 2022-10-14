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

#### useEffect / useLayoutEffect

`userEffect`와 `userLayoutEffect` 둘 다 <b>side effect</b>를 수행하기 위해 사용되고 선택적으로 cleanup function을 반환합니다. 이것은 만약 이 hook들이 반환 값을 처리하지 않는다면, type이 필요 없다는 뜻입니다. `useEffect`를 사용할 때, 함수 또는 `undefined` 이외의 다른 것을 반환하지 않도록 주의하세요. 그렇지 않으면 TypeScript와 React는 당신에게 비명을 지를것입니다. Arros functions를 사용한다면 이 문제는 다소 파악하기 어려울 수 있습니다. :

```ts
function DelayedEffect(props: { timerMs: number }) {
  const { timerMs } = props;

  useEffect(
    () =>
      setTimeout(() => {
        /* do stuff */
      }, timerMs),
    [timerMs]
  );
  // 나쁜 예시! setTimeout은 암묵적으로 숫자를 반환하고 있습니다.
  // arrow function의 body가 중괄호로 감싸지지 않았기 때문입니다.
  return null;
}
```

<details>
<summary><b>위 예시에 대한 해결책</b></summary>

```tsx
function DelayedEffect(props: { timerMs: number }) {
  const { timerMs } = props;

  useEffect(() => {
    setTimeout(() => {
      /* do stuff */
    }, timerMs);
  }, [timerMs]);
  // 더 나은 방법; 확실하게 undefined를 반환하기 위해서 void keyword를 사용하세요.
  return null;
}
```

</details>

#### useRef

TypeScript에서 `useRef`는 type argument가 초기 값을 완전히 포함(cover)하는지 아닌지에 따라[read-only](https://github.com/DefinitelyTyped/DefinitelyTyped/blob/abd69803c1b710db58d511f4544ec1b70bc9077c/types/react/v16/index.d.ts#L1025-L1039)또는 [mutable](https://github.com/DefinitelyTyped/DefinitelyTyped/blob/abd69803c1b710db58d511f4544ec1b70bc9077c/types/react/v16/index.d.ts#L1012-L1023) 둘 중 하나를 반환합니다. 각자의 use case에 맞는 것을 선택하세요.

##### Option 1: DOM element ref

**[DOM element에 접근하기 위해서는](https://reactjs.org/docs/refs-and-the-dom.html):** element type 만을 argument로 넘겨주고 `null`을 초기 값으로 사용하세요. 이 경우에, 반환되는 reference는 React에 의해 관리되는 read-only `.current`를 가질 것입니다. TypeScript는 이 ref를 element의 `ref` prop으로 전달 받기를 기대합니다. :

```tsx
function Foo() {
  // - 가능한 상세하게 작성하세요. 예를들면, HTMLDivElement는 HTMLElement보다 더 좋고,
  // Element보다는 훨신 더 좋은 선택입니다.
  // - 기술적으로 말하자면, 이것은 RefObject<HTMLDivElement>를 반환합니다.
  const divRef = useRef<HTMLDivElement>(null);

  useEffect(() => {
    // ref.current가 null일 수 있다는 것을 주의하세요.
    // 이것은 당신이 조건에 따라서 ref된(ref-ed) element를 render하거나
    // 할당하는 것을 잊을 수 있기 때문에 예측할 수 있는 현상입니다.
    if (!divRef.current) throw Error("divRef is not assigned");

    // 이제 divRef.current는 확실하게 HTMLDivElement 입니다.
    doSomethingWith(divRef.current);
  });

  // React가 당신을 위해 ref를 관리할 수있도록 element에게 ref를 전달해 주세요.
  return <div ref={divRef}>etc</div>;
}
```

만약 `divRef.current`가 절대로 null이 아닐것이라는 것을 확신한다면, non-null assertion operator `!`을 사용하는 것도 가능합니다. :

```tsx
const divRef = useRef<HTMLDivElement>(null!);
// 나중에... 이것이 null 인지 확인할 필요가 없습니다.
doSomethingWith(divRef.current);
```

당신이 type safety가 보장된다고 미리 가정하고 코드를 작성한다는 것에 주의해야 합니다. 렌더링 과정에서 ref를 element에 할당하는 것을 잊거나, ref된(ref-ed) element가 조건부 렌더링 된다면 runtime error가 발생할 것입니다.

<details>
<summary><b>Tip: 어떤 <code>HTMLElement</code>를 사용할지 선택하기</b></summary>
  
Ref는 명시성(specificity)을 필요로 합니다. 즉, `HTMLElement` 만을 명시하는 것은 충분하지 않다는 말입니다. 만약 당신이 필요한 element type의 이름을 모른다면, [lib.dom.ts](https://github.com/microsoft/TypeScript/blob/v3.9.5/lib/lib.dom.d.ts#L19224-L19343)에서 확인하거나 의도적으로 type error를 발생시키고 language service가 type의 이름을 알려주도록 할 수 있습니다.

![image](https://user-images.githubusercontent.com/6764957/116914284-1c436380-ac7d-11eb-9150-f52c571c5f07.png)

</details>

##### Option 2: Mutable value ref

**[mutable value를 가지기 위해서는](https://reactjs.org/docs/hooks-faq.html#is-there-something-like-instance-variables):** 원하는 type을 사용하고 초기 값이 완전히 해당 type에 속하는지 확인하세요.

```tsx
function Foo() {
  // 기술적으로 말하자면, 이것은 MutableRefObject<number | null>을 반환합니다.
  const intervalRef = useRef<number | null>(null);

  // 당신이 직접 ref를 관리합니다. (이것이 MutableRefObject라고 불리는 이유이죠.)
  useEffect(() => {
    intervalRef.current = setInterval(...);
    return () => clearInterval(intervalRef.current);
  }, []);

  // ref는 element의 "ref" prop으로 전달되지 않습니다.
  return <button onClick={/* clearInterval the ref */}>Cancel timer</button>;
}
```

##### 다음의 자료도 확인해 보세요.

- [@rajivpunjabi가 작성한 관련 이슈](https://github.com/typescript-cheatsheets/react/issues/388) - [Playground](https://www.typescriptlang.org/play#code/JYWwDg9gTgLgBAKjgQwM5wEoFNkGN4BmUEIcARFDvmQNwCwAUI7hAHarwCCYYcAvHAAUASn4A+OAG9GjOHAD0CBLLnKGcxHABiwKBzgQwMYGxS4WUACbBWAczgwIcSxFwBXEFlYxkxtgDoVTQBJVmBjZAAbOAA3KLcsOAB3YEjogCNE1jc0-zgAGQBPG3tHOAAVQrAsAGVcKGAjOHTCuDdUErhWNgBabLSUVFQsWBNWA2qoX2hA9VU4AGFKXyx0AFk3H3TIxOwCOAB5dIArLHwgpHcoSm84MGJJmFbgdG74ZcsDVkjC2Y01f7yFQsdjvLAEACM-EwVBg-naWD2AB4ABLlNb5GpgZCsACiO083jEgn6kQAhMJ6HMQfpKJCFpE2IkBNg8HCEci0RisTj8VhCTBiaSKVSVIoAaoLnBQuFgFFYvFEikBpkujkMps4FgAB7VfCdLmY7F4gleOFwAByEHg7U63VYfXVg2Go1MhhG0ygf3mAHVUtF6jgYLtwUdTvguta4Bstjs9mGznCpVcbvB7u7YM90B8vj9vYgLkDqWxaeCAEzQ1n4eHDTnoo2801EknqykyObii5SmpnNifA5GMZmCzWOwOJwudwC3xjKUyiLROKRBLJf3NLJO9KanV64xj0koVifQ08k38s1Sv0DJZBxIx5DbRGhk6J5Nua5mu4PEZPOAvSNgsgnxsHmXZzIgRZyDSYIEAAzJWsI1k+BCovWp58gKcAAD5qmkQqtqKHbyCexoYRecw7IQugcAs76ptCdIQv4KZmoRcjyMRaGkU28A4aSKiUXAwwgpYtEfrcAh0mWzF0ax7bsZx3Lceetx8eqAlYPAMAABa6KJskSXAdKwTJ4kwGxCjyKy-bfK05SrDA8mWVagHAbZeScOY0CjqUE6uOgqDaRAOSfKqOYgb8KiMaZ9GSeCEIMkyMVyUwRHWYc7nSvAgUQEk6AjMQXpReWyWGdFLHeBZHEuTCQEZT8xVwaV8BxZCzUWZQMDvuMghBHASJVnCWhTLYApiH1chIqgxpGeCfCSIxAC+Yj3o+8YvvgSLyNNOLjeBGhTTNdLzVJy3reGMBbTtrB7RoB3XbNBAneCsHLatcbPhdV3GrdB1WYhw3IKNZq-W2DCLYRO7QPAljgsgORcDwVJAA)
- [Stefan Baumgartner의 예시](https://fettblog.eu/typescript-react/hooks/#useref) - [Playground](https://www.typescriptlang.org/play/?jsx=2#code/JYWwDg9gTgLgBAJQKYEMDG8BmUIjgIilQ3wFgAoCzAVwDsNgJa4AVJADxgElaxqYA6sBgALAGIQ01AM4AhfjCYAKAJRwA3hThwA9DrjBaw4CgA2waUjgB3YSLi1qp0wBo4AI35wYSZ6wCeYEgAymhQwGDw1lYoRHCmEBAA1oYA5nCY0HAozAASLACyADI8fDAAoqZIIEi0MFpwaEzS8IZllXAAvIjEMAB0MkjImAA8+cWl-JXVtTAAfEqOzioA3A1NtC1wTPIwirQAwuZoSV1wql1zGg3aenAt4RgOTqaNIkgn0g5ISAAmcDJvBA3h9TsBMAZeFNXjl-lIoEQ6nAOBZ+jddPpPPAmGgrPDEfAUS1pG5hAYvhAITBAlZxiUoRUqjU6m5RIDhOi7iIUF9RFYaqIIP9MlJpABCOCAUHJ0eDzm1oXAAGSKyHtUx9fGzNSacjaPWq6Ea6gI2Z9EUyVRrXV6gC+DRtVu0RBgxuYSnRIzm6O06h0ACpIdlfr9jExSQyOkxTP5GjkPFZBv9bKIDYSmbNpH04ABNFD+CV+nR2636kby+BETCddTlyo27w0zr4HycfC6L0lvUjLH7baHY5Jas7BRMI7AE42uYSUXed6pkY6HtMDulnQruCrCg2oA)

#### useImperativeHandle

해당 [Stackoverflow answer](https://stackoverflow.com/a/69292925/5415299)에 따르면 다음과 같습니다.:

```tsx
// Countdown.tsx

// forwardRef로 전달될 handle type을 정의합니다
export type CountdownHandle = {
  start: () => void;
};

type CountdownProps = {};

const Countdown = forwardRef<CountdownHandle, CountdownProps>((props, ref) => {
  useImperativeHandle(ref, () => ({
    // start() 는 여기서 타입 추론(type inference) 됩니다
    start() {
      alert("Start");
    },
  }));

  return <div>Countdown</div>;
});
```

```tsx
// 이 컴포는트는 Countdown 컴포넌트를 사용합니다

import Countdown, { CountdownHandle } from "./Countdown.tsx";

function App() {
  const countdownEl = useRef<CountdownHandle>(null);

  useEffect(() => {
    if (countdownEl.current) {
      // start()는 여기서도 타입 추론(type inference) 됩니다.
      countdownEl.current.start();
    }
  }, []);

  return <Countdown ref={countdownEl} />;
}
```

##### 다음의 자료도 확인해보세요:

- [ForwardRefRenderFunction 사용하기](https://stackoverflow.com/a/62258685/5415299)

#### Custom Hooks

만약 Custom Hook에서 array를 return한다면, array의 각 위치에서 각기 다른 type을 가지기를 원하겠지만 TypeScript는 union type으로 추론할 것이기 때문에 타입 추론을 피하고 싶을 것입니다. 이러한 상황에서 [TS 3.4 const assertions](https://devblogs.microsoft.com/typescript/announcing-typescript-3-4/#const-assertions)을 사용할 수 있습니다.

```tsx
import { useState } from "react";

export function useLoading() {
  const [isLoading, setState] = useState(false);
  const load = (aPromise: Promise<any>) => {
    setState(true);
    return aPromise.finally(() => setState(false));
  };
  return [isLoading, load] as const; // (boolean | typeof load)[]이 아닌 [boolean, typeof load]으로 추론합니다.
}
```

[TypeScript Playground에서 확인해 보기](https://www.typescriptlang.org/play/?target=5&jsx=2#code/JYWwDg9gTgLgBAJQKYEMDG8BmUIjgcilQ3wFgAoCpAD0ljkwFcA7DYCZuRgZyQBkIKACbBmAcwAUASjgBvCnDhoO3eAG1g3AcNFiANHF4wAyjBQwkAXTgBeRMRgA6HklPmkEzCgA2vKQG4FJRV4b0EhWzgJFAAFHBBNJAAuODjcRIAeFGYATwA+GRs8uSDFIzcLCRgoRiQA0rgiGEYoTlj4xMdMUR9vHIlpW2Lys0qvXzr68kUAX0DpxqRm1rgNLXDdAzDhaxRuYOZVfzgAehO4UUwkKH21ACMICG9UZgMYHLAkCEw4baFrUSqVARb5RB5PF5wAA+cHen1BfykaksFBmQA)

이런 방법으로, destructure했을 때 destructureg한 위치에 따라 올바른 type을 얻을 수 있습니다.

<details>
<summary><b>대안: tuple return type을 표명하기(assert)</b></summary>

만약 [const assertions이 사용하기 어렵다면](https://github.com/babel/babel/issues/9800), 함수 return type을 표명(assert)하거나 정의할 수 있습니다.

```tsx
import { useState } from "react";

export function useLoading() {
  const [isLoading, setState] = useState(false);
  const load = (aPromise: Promise<any>) => {
    setState(true);
    return aPromise.finally(() => setState(false));
  };
  return [isLoading, load] as [boolean, (aPromise: Promise<any>) => Promise<any>];
}
```

많은 custom hooks을 작성한다면, 자동으로 tuples의 타입을 명시해주는 helper도 큰 도움이 될 수 있습니다.

```tsx
function tuplify<T extends any[]>(...elements: T) {
  return elements;
}

function useArray() {
  const numberValue = useRef(3).current;
  const functionValue = useRef(() => {}).current;
  return [numberValue, functionValue]; // type is (number | (() => void))[]
}

function useTuple() {
  const numberValue = useRef(3).current;
  const functionValue = useRef(() => {}).current;
  return tuplify(numberValue, functionValue); // type is [number, () => void]
}
```

</details>

하지만 React team은 두개 이상의 값을 return하는 custom hook은 tuple 대신 적절한 object를 사용하는 것을 권장한다는 것에 주의하세요.

#### 더 많은 Hooks + TypeScript 에 관한 읽을 거리:

- https://medium.com/@jrwebdev/react-hooks-in-typescript-88fce7001d0d
- https://fettblog.eu/typescript-react/hooks/#useref

만약 React Hooks library를 작성하고 있다면, 사용자들이 사용할 수 있도록 types를 export 해야 한다는 것을 잊지 마세요.

#### React Hooks + TypeScript Libraries 예시:

- https://github.com/mweststrate/use-st8
- https://github.com/palmerhq/the-platform
- https://github.com/sw-yx/hooks

[추가할 내용이 있나요? issue를 장성하세요!](https://github.com/typescript-cheatsheets/react/issues/new).

<!--END-SECTION:hooks-->

<!--START-SECTION:class-components-->

#### Class Components

TypeScript에서 `React.Component`는 generic type (aka `React.Component<PropType, StateType>`)입니다. 따라서 `React.Component`에 prop과 state type parameter를 전달해야 합니다. :

```tsx
type MyProps = {
  // `interface`를 사용하는 것도 괜찮습니다
  message: string;
};
type MyState = {
  count: number; // 이런 식으로
};
class App extends React.Component<MyProps, MyState> {
  state: MyState = {
    // 더 나은 타입 추론을 위해 선택적으로 작성한 두 번째 annotation
    count: 0,
  };
  render() {
    return (
      <div>
        {this.props.message} {this.state.count}
      </div>
    );
  }
}
```

[TypeScript Playground 확인해 보기](https://www.typescriptlang.org/play/?jsx=2#code/JYWwDg9gTgLgBAJQKYEMDG8BmUIjgcilQ3wFgAoCmATzCTgFlqAFHMAZzgF44BvCuHAD0QuAFd2wAHYBzOAANpMJFEzok8uME4oANuwhwIAawFwQSduxQykALjjsYUaTIDcFAL4fyNOo2oAZRgUZW4+MzQIMSkYBykxEAAjFTdhUV1gY3oYAAttLx80XRQrOABBMDA4JAAPZSkAE05kdBgAOgBhXEgpJFiAHiZWCA4AGgDg0KQAPgjyQSdphyYpsJ5+BcF0ozAYYAgpPUckKKa4FCkpCBD9w7hMaDgUmGUoOD96aUwVfrQkMyCKIxOJwAAMZm8ZiITRUAAoAJTzbZwIgwMRQKRwOGA7YDRrAABuM1xKN4eW07TAbHY7QsVhsSE8fAptKWynawNinlJcAGQgJxNxCJ8gh55E8QA)

재사용하기 위해 이러한 types/interfaces를 export/import/extend 할 수 있다는 것을 잊지 마세요.

<details>
<summary><b>왜 <code>state</code>를 두 번 annotate 할까요?</b></summary>

반드시 `state` class property에 annotate할 필요는 없지만, 이렇게 하면 `this.state`에 접근하거나 state를 초기화 할 때 더 나은 타입 추론을 가능하게 합니다.

그 이유는 두 개의 annotation은 서로 다른 방식으로 동작하기 때문입니다. 두 번째 generic type parameter는 `this.setState()`가 올바르게 동작하도록 해줍니다. 왜냐하면 이 메소드는 base class에서 오기 때문입니다. 하지만 컴포넌트 내에서 `state`를 초기화 하는 것은 base implementation을 override하기 때문에 컴파일러에게 사실상 다른 작업을 하고 있지 않다는 것을 알려줘야 합니다. (=컴파일러에게 사실상 같은 작업을 하고 있다는 것을 알려줘야 합니다.)

[여기서 @ferdaber의 의견을 확인해보세요](https://github.com/typescript-cheatsheets/react/issues/57).

</details>

<details>
  <summary><b><code>readonly</code>는 필요 없다</b></summary>

종종 샘플 코드에 props와 state가 변할 수 없다고 표시하기 위해 `readonly`를 포합하는 것을 볼 수 있습니다.

```tsx
type MyProps = {
  readonly message: string;
};
type MyState = {
  readonly count: number;
};
```

`React.Component<P,S>`가 이미 props와 state가 변할 수 없다고 표시했기 때문에 추가적으로 readonly표시를 할 필요가 없습니다. ([PR 과 discussion을 확인하세요!](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/26813))

</details>

**Class Methods**: 원래 하던데로 하되, 당신의 함수를 위한 모든 arguments는 type이 있어야 한다는 것만 기억하세요.

```tsx
class App extends React.Component<{ message: string }, { count: number }> {
  state = { count: 0 };
  render() {
    return (
      <div onClick={() => this.increment(1)}>
        {this.props.message} {this.state.count}
      </div>
    );
  }
  increment = (amt: number) => {
    // 이런 식으로
    this.setState((state) => ({
      count: state.count + amt,
    }));
  };
}
```

[TypeScript Playground에서 확인해 보기](https://www.typescriptlang.org/play/?jsx=2#code/JYWwDg9gTgLgBAJQKYEMDG8BmUIjgcilQ3wFgAoCtAGxQGc64BBMMOJADxiQDsATRsnQwAdAGFckHrxgAeAN5wQSBigDmSAFxw6MKMB5q4AXwA0cRWggBXHjG09rIAEZIoJgHwWKcHTBTccAC8FnBWtvZwAAwmANw+cET8bgAUAJTe5L6+RDDWUDxwKQnZcLJ8wABucBA8YtTAaADWQfLpwV4wABbAdCIGaETKdikAjGnGHiWlFt29ImA4YH3KqhrGsz19ugFIIuF2xtO+sgD0FZVTWdlp8ddH1wNDMsFFKCCRji5uGUFe8tNTqc4A0mkg4HM6NNISI6EgYABlfzcFI7QJ-IoA66lA6RNF7XFwADUcHeMGmxjStwSxjuxiAA)

**Class Properties**: 만약 나중에 사용하기 위해 class properties를 선언한다면, `state`와 같이 선언하되 할당은 하지 안습니다.

```tsx
class App extends React.Component<{
  message: string;
}> {
  pointer: number; // 이런 식으로
  componentDidMount() {
    this.pointer = 3;
  }
  render() {
    return (
      <div>
        {this.props.message} and {this.pointer}
      </div>
    );
  }
}
```

[TypeScript Playground에서 확인해 보기](https://www.typescriptlang.org/play/?jsx=2#code/JYWwDg9gTgLgBAJQKYEMDG8BmUIjgcilQ3wFgAoCtAGxQGc64BBMMOJADxiQDsATRsnQwAdAGFckHrxgAeAN4U4cEEgYoA5kgBccOjCjAeGgNwUAvgD44i8sshHuUXTwCuIAEZIoJuAHo-OGpgAGskOBgAC2A6JTg0SQhpHhgAEWA+AFkIVxSACgBKGzjlKJiRBxTvOABeOABmMzs4cziifm9C4ublIhhXKB44PJLlOFk+YAA3S1GxmzK6CpwwJdV1LXM4FH4F6KXKp1aesdk-SZnRgqblY-MgA)

[추가할 내용이 있나요? issue를 생성하세요!](https://github.com/typescript-cheatsheets/react/issues/new).

#### getDerivedStateFromProps 타입핑(Typing) 하기

`getDerivedStateFromProps`를 사용하기 전에, [documentation](https://reactjs.org/docs/react-component.html#static-getderivedstatefromprops)과 [You Probably Don't Need Derived State](https://reactjs.org/blog/2018/06/07/you-probably-dont-need-derived-state.html)를 읽어보세요. Derived State는 memoization을 설정한는 것을 도울 수 있는 hooks을 사용하여 구현될 수 있습니다.

다음은 `getDerivedStateFromProps`를 annotate할 수 있는 몇 가지 방법입니다.

1. 만약 derived state의 type을 명시적으로 설정했고, `getDerivedStateFromProps`의 return 값이 설정한 type을 준수하는지 알고싶은 경우

```tsx
class Comp extends React.Component<Props, State> {
  static getDerivedStateFromProps(props: Props, state: State): Partial<State> | null {
    //
  }
}
```

2. 함수의 return 값이 state를 결정하도록 하고싶은 경우

```tsx
class Comp extends React.Component<Props, ReturnType<typeof Comp["getDerivedStateFromProps"]>> {
  static getDerivedStateFromProps(props: Props) {}
}
```

3. 다른 state fields와 derived state 그리고 memoization을 원할 경우

```tsx
type CustomValue = any;
interface Props {
  propA: CustomValue;
}
interface DefinedState {
  otherStateField: string;
}
type State = DefinedState & ReturnType<typeof transformPropsToState>;
function transformPropsToState(props: Props) {
  return {
    savedPropA: props.propA, // save for memoization
    derivedState: props.propA,
  };
}
class Comp extends React.PureComponent<Props, State> {
  constructor(props: Props) {
    super(props);
    this.state = {
      otherStateField: "123",
      ...transformPropsToState(props),
    };
  }
  static getDerivedStateFromProps(props: Props, state: State) {
    if (isEqual(props.propA, state.savedPropA)) return null;
    return transformPropsToState(props);
  }
}
```

[TypeScript Playground에서 확인해 보기](https://www.typescriptlang.org/play/?jsx=2#code/JYWwDg9gTgLgBAJQKYEMDG8BmUIjgcilQ3wFgAoUSWOYAZwFEBHAVxQBs5tcD2IATFHQAWAOnpJWHMuQowAnmCRwAwizoxcANQ4tlAXjgoAdvIDcFYMZhIomdMoAKOMHTgBvCnDhgXAQQAuVXVNEB12PQtyAF9La1t7NGUAESRMKyR+AGUYFBsPLzgIGGFbHLykADFgJHZ+II0oKwBzKNjyBSU4cvzDVPTjTJ7lADJEJBgWKGMAFUUkAB5OpAhMOBgoEzpMaBBnCFcZiGGAPijMFmMMYAhjdc3jbd39w+PcmwAKXwO6IJe6ACUBXI3iIk2mwO83joKAAbpkXoEfC46KJvmA-AAaOAAehxcBh8K40DgICQIAgwAAXnkbsZCt5+LZgPDsu8kEF0aj0X5CtE2hQ0OwhG4VLgwHAkAAPGzGfhuZDoGCiRxTJBi8C3JDWBb-bGnSFwNC3RosDDQL4ov4ooGeEFQugsJRQS0-AFRKHrYT0UQaCpwQx2z3eYqlKDDaq1epwABEAEYAEwAZhjmIZUNEmY2Wx2UD2KKOw1drgB6f5fMKfpgwDQcGaE1STVZEZw+Z+xd+cD1BPZQWGtvTwDWH3ozDY7A7aP82KrSF9cIR-gBQLBUzuxhY7HYHqhq4h2ceubbryLXPdFZiQA)

<!--END-SECTION:class-components-->

<!--START-SECTION:default-props-->

#### `defaultProps`가 필요하지 않을수도 있습니다

[이 트윗](https://twitter.com/dan_abramov/status/1133878326358171650)에 따르면, defaultProps는 deprecate 될 것입니다.. 다음의 토론을 확인해 보세요.:

- [Original tweet](https://twitter.com/hswolff/status/1133759319571345408)
- [이 article](https://medium.com/@matanbobi/react-defaultprops-is-dying-whos-the-contender-443c19d9e7f1)에서 더 많은 정보를 얻을 수 있습니다.

object default value를 사용하는 것이 통상적으로 합의된 내용입니다.

Function Components:

```tsx
type GreetProps = { age?: number };

const Greet = ({ age = 21 }: GreetProps) => // etc
```

Class Components:

```tsx
type GreetProps = {
  age?: number;
};

class Greet extends React.Component<GreetProps> {
  render() {
    const { age = 21 } = this.props;
    /*...*/
  }
}

let el = <Greet age={3} />;
```

#### `defaultProps` 타이핑 하기

[TypeScript 3.0+](https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-0.html)에서 타입 추론의 성능이 매우 많이 발전되었습니다. 하지만 여전히 [몇몇의 edge case 들이 문제가 되기는 합니다.](https://github.com/typescript-cheatsheets/react/issues/61).

**Function Components**

```tsx
// 쉬운 방법으로 typeof를 사용할 수 있습니다.; hoist되는 것에 주의하세요!
// DefaultProps을 선언할 수도 있습니다.
// e.g. https://github.com/typescript-cheatsheets/react/issues/415#issuecomment-841223219
type GreetProps = { age: number } & typeof defaultProps;

const defaultProps = {
  age: 21,
};

const Greet = (props: GreetProps) => {
  // etc
};
Greet.defaultProps = defaultProps;
```

_[TS Playground에서 확인해보기](https://www.typescriptlang.org/play?#code/JYWwDg9gTgLgBAKjgQwM5wEoFNkGN4BmUEIcARFDvmQNwBQdMAnmFnAOKVYwAKxY6ALxwA3igDmWAFxwAdgFcQAIyxQ4AXzgAyOM1YQCcACZYCyeQBte-VPVwRZqeCbOXrEAXGEi6cCdLgAJgBGABo6dXo6e0d4TixuLzgACjAbGXjuPg9UAEovAD5RXzhKGHkoWTgAHiNgADcCkTScgDpkSTgAeiQFZVVELvVqrrrGiPpMmFaXcytsz2FZtwXbOiA)_

**Class components**의 경우, 타이핑을 위한 [두 가지 방법](https://github.com/typescript-cheatsheets/react/pull/103#issuecomment-481061483) (including using the `Pick` utility type)이 있지만, props definition을 거꾸로 수행("reverse") 하는 것을 추천합니다.

```tsx
type GreetProps = typeof Greet.defaultProps & {
  age: number;
};

class Greet extends React.Component<GreetProps> {
  static defaultProps = {
    age: 21,
  };
  /*...*/
}

// Type-checks! type assertion이 필요 없음!
let el = <Greet age={3} />;
```

<details>
<summary>라이브러리 작성자를 위한<b><code>JSX.LibraryManagedAttributes</code> 뉘앙스</b></summary>

위에서 소개된 구현은 앱 개발자들이 사용하는데 아무런 문제가 없습니다. 하지만 다른 사람들이 사용(consume)할 수 있도록 `GreetProps`를 export 하고싶은 경우도 있습니다. 여기서 `GreetProps`가 정의되는 방법이 문제가 됩니다. `age`는 꼭 필요하지 않을 때에도 `defaultProps`때문에 필수적인 props가 됩니다.

[`GreetProps`는 당신의 컴포넌트를 위한 _내부적인_ 규칙(컴포넌트가 구현하는 것)이지, _외부적인_ 것이 아닙니다](https://github.com/typescript-cheatsheets/react/issues/66#issuecomment-453878710). 따라서 export를 위한 type을 따로 만들 거나, `JSX.LibraryManagedAttributes` utility를 사용할 수도 있습니다.

```tsx
// internal contract(내부적인 규칙), export 되어서는 안된다
type GreetProps = {
  age: number;
};

class Greet extends Component<GreetProps> {
  static defaultProps = { age: 21 };
}

// external contract(외부적인 규칙)
export type ApparentGreetProps = JSX.LibraryManagedAttributes<typeof Greet, GreetProps>;
```

이렇게 하면 코드가 잘 실행되지만, `ApparentGreetProps`를 사용하는게 다소 번거로울 수 있습니다. 아래에서 설명하는 `ComponentProps` utility로 boilerplate를 간단하게 만들 수 있습니다.

</details>

#### defaultProps가 있는 Component의 props를 사용(consume)하기

`defaultProps`가 있는 컴포넌트는 실제로는 그렇지 않지만 필수적인 props를 가지는 것처럼 보일 수 있습니다.

##### Problem Statement

다음과 같은 작업을 하고싶다면,

```tsx
interface IProps {
  name: string;
}
const defaultProps = {
  age: 25,
};
const GreetComponent = ({ name, age }: IProps & typeof defaultProps) => (
  <div>{`Hello, my name is ${name}, ${age}`}</div>
);
GreetComponent.defaultProps = defaultProps;

const TestComponent = (props: React.ComponentProps<typeof GreetComponent>) => {
  return <h1 />;
};

// 'age' property는 '{ name: string; }'에 없지만, '{ age: number; } type에서는 필수적인 property 입니다.
const el = <TestComponent name="foo" />;
```

##### Solution

`JSX.LibraryManagedAttributes`를 적용하는 유틸리티를 정의합니다.

```tsx
type ComponentProps<T> = T extends React.ComponentType<infer P> | React.Component<infer P>
  ? JSX.LibraryManagedAttributes<T, P>
  : never;

const TestComponent = (props: ComponentProps<typeof GreetComponent>) => {
  return <h1 />;
};

// No error
const el = <TestComponent name="foo" />;
```

[_TS Playground에서 확인해 보기_](https://www.typescriptlang.org/play?#code/JYWwDg9gTgLgBAKjgQwM5wEoFNkGN4BmUEIcARFDvmQNwBQdMAnmFnAMImQB2W3MABWJhUAHgAqAPjgBeOOLhYAHjD4ATdNjwwAdJ3ARe-cSyyjg3AlihwB0gD6Yqu-Tz4xzl67cl04cAH44ACkAZQANHQAZYAAjKGQoJgBZZG5kAHMsNQBBGBgoOIBXVTFxABofPzgALjheADdrejoLVSgCPDYASSEIETgAb2r0kCw61AKLDPoAXzpcQ0m4NSxOooAbQWF0OWH-TPG4ACYAVnK6WfpF7mWAcUosGFdDd1k4AApB+uQxysO4LM6r0dnAAGRwZisCAEFZrZCbbb9VAASlk0g+1VEamADUkgwABgAJLAbDYQSogJg-MZwYDoAAkg1GWFmlSZh1mBNmogA9Di8XQUfQHlgni8jLpVustn0BnJpQjZTsWrzeXANsh2gwbstxFhJhK3nIPmAdnUjfw5WIoVgYXBReKuK9+JI0TJpPs4JQYEUoNw4KIABYARjgvN8VwYargADkIIooMQoAslvBSe8JAbns7JTSsDIyAQIBAyOHJDQgA)

#### 여러가지 토론과 지식

<details>
<summary><b><code>React.FC</code>는 왜 <code>defaultProps</code>이 동작하지 못하게 만들까요?</b></summary>

다음의 토론을 확인해 보세요.:

- https://medium.com/@martin_hotell/10-typescript-pro-tips-patterns-with-or-without-react-5799488d6680
- https://github.com/DefinitelyTyped/DefinitelyTyped/issues/30695
- https://github.com/typescript-cheatsheets/react/issues/87

이건 현재 상태일 뿐이고, 추후에는 올바르게 수정될 것입니다.

</details>

<details>
<summary><b>TypeScript 2.9 and earlier</b></summary>

TypeScript 2.9와 그 이전 버전에서는 이문제를 해결하는 방법이 다양합니다. 하지만 다음 방법이 여태까지 확인한 방법 중 가장 좋은 방법입니다.

```ts
type Props = Required<typeof MyComponent.defaultProps> & {
  /* 추가적인 props */
};

export class MyComponent extends React.Component<Props> {
  static defaultProps = {
    foo: "foo",
  };
}
```

이전에는 TypeScript의 `Partial type` 기능을 사용하는 것이 권장 사항이었는데, 이는 현재 인터페이스가 래핑된 인터페이스에에서 부분적인 버전을 충족한다는 것을 의미합니다. 이런 방법으로 type을 변경하지 않고 defaultProps를 확장할 수 있습니다.

```ts
interface IMyComponentProps {
  firstProp?: string;
  secondProp: IPerson[];
}

export class MyComponent extends React.Component<IMyComponentProps> {
  public static defaultProps: Partial<IMyComponentProps> = {
    firstProp: "default",
  };
}
```

이 접근 방법의 문제점은 `JSX.LibraryManagedAttributes`로 작동하는 타입 추론에 복잡한 이슈를 발생시킨다는 것입니다. 기본적으로 컴파일러는 해당 컴포넌트로 JSX expression을 생성할 때 모든 props가 선택사항(optional)이라고 생각합니다.

[@ferdaber의 의견을 확인해 보세요.](https://github.com/typescript-cheatsheets/react/issues/57) and [here](https://github.com/typescript-cheatsheets/react/issues/61).

</details>

[추가할 내용이 있나요? 이슈를 생성하세요!](https://github.com/typescript-cheatsheets/react/issues/new).

<!--END-SECTION:default-props-->
