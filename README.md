# React+TypeScript Cheatsheets ํ๊ตญ์ดํ ๐ฐ๐ท

TypeScript์ ์๋ฌธํ๋ React ๊ฐ๋ฐ์๋ฅผ ์ํ ์นํธ์ํธ(Cheetsheets)

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

[**์น ๋คํ๋จผํธ**](https://react-typescript-cheatsheet.netlify.app/docs/basic/setup) |
[**์์ดํ**](https://github.com/typescript-cheatsheets/react-typescript-cheatsheet-es) |
[ํ๋ก์ ํธ์ ๊ธฐ์ฌํ๊ธฐ]() |
[์ง๋ฌธํ๊ธฐ]()

:wave: ๋ณธ ๋ฆฌํฌ์งํ ๋ฆฌ๋ [@ryan_kim_kr](https://twitter.com/ryan_kim_kr)์ ์ํด ๊ด๋ฆฌ๋๊ณ  ์์ต๋๋ค. ๊ฐ๋ฐ์๋์ด React์ ํจ๊ป TypeScript๋ฅผ ์ฌ์ฉํด๋ณด๊ณ ์ ํ์๋ค๋ ์ ๋ง ๊ธฐ์ ์์์ด๊ตฐ์! ์๋ชป๋ ๋ถ๋ถ์ด ๋ฐ๊ฒฌ๋์ด ์์ ์ด ํ์ํ๊ฑฐ๋ ๋๋ฝ๋ ๋ถ๋ถ์ด ์๋ค๋ฉด ๊ฐ์  ๋์ด์ผ ํ  ์ฌํญ์ [์ด์ ๋ฑ๋ก](https://github.com/typescript-cheatsheets/react-typescript-cheatsheet-kr/issues/new)ํด ์ฃผ์๊ธฐ ๋ฐ๋๋๋ค. :+1:

---

[![All Contributors](https://img.shields.io/github/contributors/typescript-cheatsheets/react-typescript-cheatsheet?color=orange&style=flat-square)](/COLABORADORES.md)

# All React + TypeScript Cheatsheets

- [๊ธฐ์ด ์นํธ์ํธ(The Basic Cheatsheet)]()๋ React ๊ฐ๋ฐ์๊ฐ React app์์ TS ์ฌ์ฉ์ ์์ํ๋ ๊ฒ์ ๋์์ ์ฃผ๊ธฐ ์ํ ๋ด์ฉ์ด ์ฃผ๋ฅผ ์ด๋ฃน๋๋ค.
  - ๋ชจ๋ฒ ์ฌ๋ก(Best Practices)๋ผ๊ณ  ์ฌ๊ฒจ์ง๋, ๋ณต์ฌ + ๋ถ์ฌ๋ฃ๊ธฐ ๊ฐ๋ฅํ ์์
  - ๊ธฐ๋ณธ์ ์ธ TS Types ์ฌ์ฉ๋ฒ๊ณผ ์ค์  ๋ฐฉ๋ฒ
  - ์์ฃผ ๋ฌป๋ ์ง๋ฌธ(FAQ)์ ๋ํ ๋ต๋ณ
  - Generic type logic์ ๊น์ด ๋ค๋ฃจ์ง ์์ต๋๋ค. ๊ทธ ๋์ , ์ด์ฌ์๋ค์ ์ํด ๊ฐ๋จํ ํธ๋ฌ๋ธ์ํ ๊ธฐ์ ๋ค์ ์๊ฐํฉ๋๋ค.
  - ๊ธฐ์ด ์นํธ์ํธ๋ ๊ฐ๋ฐ์๊ฐ TypeScript์ ๋ํด ๋๋ฌด ๋ง์ ๊ณต๋ถ๋ฅผ ํ์ง ์๊ณ ์๋ **์๊ฐ ํจ์จ์ **์ผ๋ก React ๊ฐ๋ฐ์ TypeScript๋ฅผ ๋น ๋ฅด๊ฒ ์ฌ์ฉํ  ์ ์๋๋ก ๋๋ ๋ฐ ๊ทธ ๋ชฉ์ ์ด ์์ต๋๋ค.
- [๊ณ ๊ธ ์นํธ์ํธ(The Advanced Cheatsheet)]()๋ ์ฌ์ฌ์ฉ ๊ฐ๋ฅํ type utilities/functions/render prop/higher order copmonents ๋๋ TS+React ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ฅผ ์์ฑํ๊ณ ์ ํ๋ ๊ฐ๋ฐ์๋ฅผ ์ํด generic types์ ๊ณ ๊ธ ์ฌ์ฉ๋ฒ์ ๋ํ ์ดํด๋ฅผ ๋์ต๋๋ค.
  - ์ ๋ฌธ์ ์ธ ๊ฐ๋ฐ์๋ค์ ์ํ ๋ค์ํ ํ๊ณผ ์๋ น๋ค์ ์๊ฐํฉ๋๋ค.
  - DefinitelyTyped์ ๊ธฐ์ฌํ๊ธฐ ์ํ ์กฐ์ธ์ ๋๋ฆฝ๋๋ค.
  - ๊ณ ๊ธ ์นํธ์ํธ๋ ๊ฐ๋ฐ์๊ฐ TypeScript๋ฅผ ์ต๋ํ ํ์ฉํ  ์ ์๋๋ก ๋๋ ๋ฐ ๊ทธ ๋ชฉ์ ์ด ์์ต๋๋ค.
- [๋ง์ด๊ทธ๋ ์ดํ ์นํธ์ํธ(The Migrating Cheatsheet)]()๋ ๋๊ท๋ชจ ์ฝ๋๋ฒ ์ด์ค๋ฅผ JS ๋๋ Flow์์ TypsScript๋ก ์ ์ง์ ์ผ๋ก ๋ง์ด๊ทธ๋ ์ด์ ํ๋ ๊ฒ์ ๋ํ ๊ฒฝํ์์ ์กฐ์ธ์ ์ป๋๋ฐ ๋์์ ์ค๋๋ค.
  - ์ฐ๋ฆฌ๋ ์ฌ๋ฌ๋ถ์ด ๋ง์ด๊ทธ๋ ์ด์์ ํ๋๋ก ์ค๋ํ๋ ค๋ ๊ฒ์ด ์๋๋ฉฐ, ์ด๋ฏธ ๊ทธ๋ ๊ฒ ํ๊ณ ์ ๊ฒฐ์ ํ ์ฌ๋๋ค์ ๋๊ณ ์ ํฉ๋๋ค.
  - โ ๏ธ ์ด ์นํธ์ํธ๋ ์๋กญ๊ฒ ๋ง๋ค์ด์ง ์นํธ์ํธ ์๋๋ค. ๋ฐ๋ผ์ ๋์์ ์ฃผ๊ณ ์ ํ๋ ๋ชจ๋  ๋ถ๋ค์ ํ์ํฉ๋๋ค.
- [HOC ์นํธ์ํธ(The HOC Cheatsheet)]()๋ ์์์ ํจ๊ป HOC๋ฅผ ์์ฑํ๋ ๋ฐฉ๋ฒ์ ์๋ ค์ค๋๋ค.
  - [Generics](https://www.typescriptlang.org/docs/handbook/2/generics.html)์ ๋ํ ์ดํด๊ฐ ์ ํ๋์ด์ผ ํฉ๋๋ค.
  - โ ๏ธ ์ด ์นํธ์ํธ๋ ์๋กญ๊ฒ ๋ง๋ค์ด์ง ์นํธ์ํธ ์๋๋ค. ๋ฐ๋ผ์ ๋์์ ์ฃผ๊ณ ์ ํ๋ ๋ชจ๋  ๋ถ๋ค์ ํ์ํฉ๋๋ค.

---

## ๊ธฐ์ด ์นํธ์ํธ (Basic Cheatsheet)

### ๊ธฐ์ด ์นํธ์ํธ ๋ชฉ์ฐจ

<details>

<summary><b>๋ชฉ์ฐจ ํ์ฅํ๊ธฐ</b></summary>

- [์น์ 1: React์ TypeScript ์ค์ ํ๊ธฐ]()
    <!--START_SECTION:setup-toc-->
  - [์ ์ ์กฐ๊ฑด]()

</details>

<!--START-SECTION:setup-->

### ์น์ 1: React์ TypeScript ์ค์ ํ๊ธฐ

#### ์์ํ๊ธฐ ์  ํ์ํ ์ฌํญ

1. [React](https://reactjs.org)์ ๋ํ ์ถฉ๋ถํ ์ดํด
2. [TypeScript Types](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html)์ฃผ์ ์ ๋ํ ์ดํด ([2ality's guide](http://2ality.com/2018/04/type-notation-typescript.html)๋ฅผ ์๊ณ ์์ผ๋ฉด ๋ฌธ์๋ฅผ ์ดํดํ๋๋ฐ ๋์์ด ๋ฉ๋๋ค. ๋ง์ฝ TypeScript๋ฅผ ์ฒ์ ์ ํ๋ ๋ถ์ด๋ผ๋ฉด,[chibicodeโs tutorial](https://ts.chibicode.com/todo/)๋ฅผ ์ฐธ๊ณ ํด ๋ณด์ธ์.)
3. [the TypeScript section in the official React docs](https://reactjs.org/docs/static-type-checking.html#typescript) ์ฝ๊ธฐ
4. [the React section of the new TypeScript playground](http://www.typescriptlang.org/play/index.html?jsx=2&esModuleInterop=true&e=181#example/typescript-with-react) ์ฝ๊ธฐ (์ ํ์ฌํญ: [the playground's](http://www.typescriptlang.org/play/index.html) Example Section์ 40+ examples ๋จ๊ณ๋ฅผ ์ํํด ๋ณด๊ธฐ)

์ด ๊ฐ์ด๋๋ ๋์๊ฐ ๊ฐ์ฅ ์ต์  ๋ฒ์ ์ TypeScript์ React๋ฅผ ์ฌ์ฉํ๋ค๊ณ  ๊ฐ์ ํฉ๋๋ค. ์ด์  ๋ฒ์ ์ ๋ํ ์ฌํญ์ ํ์ฅ ๊ฐ๋ฅํ `<details>` ํ๊ทธ๋ก ํ์ธ ๊ฐ๋ฅํฉ๋๋ค.

#### VS Code ํ์ฅ ํ๋ก๊ทธ๋จ(Extensions)

- ๋ฆฌํํ ๋ง ๋ณด์กฐ https://marketplace.visualstudio.com/items?itemName=paulshen.paul-typescript-toolkit
- R+TS Code Snippets (์ฌ๋ฌ๊ฐ์ง ํ์ฅ ํ๋ก๊ทธ๋จ์ด ์์ต๋๋ค...)
  - https://marketplace.visualstudio.com/items?itemName=infeng.vscode-react-typescript
  - https://www.digitalocean.com/community/tutorials/the-best-react-extension-for-vs-code
- TypeScript ๊ณต์ ํ์ฅํ๋ก๊ทธ๋จ https://code.visualstudio.com/docs/languages/typescript

#### React + TypeScript ์๋ฌธ์ ํคํธ

Cloud setups:

- [TypeScript Playground with React](https://www.typescriptlang.org/play?#code/JYWwDg9gTgLgBAKjgQwM5wEoFNkGN4BmUEIcA5FDvmQNwCwAUKJLHAN5wCuqWAyjMhhYANFx4BRAgSz44AXzhES5Snhi1GjLAA8W8XBAB2qeAGEInQ0KjjtycABsscALxwAFAEpXAPnaM4OANjeABtA0sYUR4Yc0iAXVcxPgEhdwAGT3oGAOTJaXx3L19-BkDAgBMIXE4QLCsAOhhgGCckgAMATQsgh2BcAGssCrgAEjYIqwVmutR27MC5LM0yuEoYTihDD1zAgB4K4AA3H13yvbAfbs5e-qGRiYspuBmsVD2Aekuz-YAjThgMCMcCMpj6gxcbGKLj8MTiVnck3gAGo4ABGTxyU6rcrlMF3OB1H5wT7-QFGbG4z6HE65ZYMOSMIA)๋ ์ฝ๋๋ฅผ ์คํํ์ง ์๊ณ  Types๋ฅผ ๋๋ฒ๊น๋ง ํ๋ ๊ฒฝ์ฐ ์ฌ์ฉํ  ์ ์์ต๋๋ค.
- [CodeSandbox](http://ts.react.new) - cloud IDE, ๋งค์ฐ ๋น ๋ฅธ ๋ถํ ์๋๋ฅผ ๊ฐ์ง๋๋ค.
- [Stackblitz](https://stackblitz.com/edit/react-typescript-base) - cloud IDE, ๋งค์ฐ ๋น ๋ฅธ ๋ถํ ์๋๋ฅผ ๊ฐ์ง๋๋ค.

Local dev setups:

- [Next.js](https://nextjs.org/docs/basic-features/typescript): `npx create-next-app -e with-typescript` ๋ช๋ น์ด๋ ์๋ก์ด NextJS ํ๋ก์ ํธ๋ฅผ ํ์ฌ ํด๋์ ์์ฑํฉ๋๋ค.
- [Create React App](https://facebook.github.io/create-react-app/docs/adding-typescript): `npx create-react-app name-of-app --template typescript` ๋ช๋ น์ด๋ ์๋ก์ด NextJS ํ๋ก์ ํธ๋ฅผ ์๋ก์ด ํด๋์ ์์ฑํฉ๋๋ค.
- [Vite](https://vitejs.dev/): `npm create vite@latest my-react-ts-app -- --template react-ts`
- [Meteor](https://guide.meteor.com/build-tool.html#typescript): `meteor create --typescript name-of-my-new-typescript-app`
- [Ignite](https://github.com/infinitered/ignite#use-ignite-andross-infinite-red-andross-boilerplate) for React Native: `ignite new myapp`
- [TSDX](https://tsdx.io/): `npx tsdx create mylib` ๋ช๋ น์ด๋ React+TS _๋ผ์ด๋ธ๋ฌ๋ฆฌ_ ๋ฅผ ์์ฑํฉ๋๋ค. (in future: [TurboRepo](https://twitter.com/jaredpalmer/status/1346217789942591488))

<details>
<summary><b>๋ค๋ฅธ ๋๊ตฌ๋ค</b></summary>

์์ง ๋ณด์์ด ํ์ํ์ง๋ง ํ์ธํด ๋ณผ ๋งํ ๊ฐ์น๊ฐ ์๋ ๋๊ตฌ๋ค:

- [Snowpack](<https://www.snowpack.dev/#create-snowpack-app-(csa)>): `npx create-snowpack-app my-app --template app-template-react-typescript`
- [Docusaurus v2](https://v2.docusaurus.io/docs/installation) with [TypeScript Support](https://v2.docusaurus.io/docs/typescript-support)
- [Parcel](https://v2.parceljs.org/languages/typescript/)
- [JP Morgan's `modular`](https://github.com/jpmorganchase/modular): CRA + TS + Yarn Workspaces toolkit. `yarn create modular-react-app <project-name>`

Manual setup:

- [Basarat's guide](https://github.com/basarat/typescript-react/tree/master/01%20bootstrap)๋ React + TypeScript + Webpack + Babel ์ **์๋์ผ๋ก ์ค์ ** ํ  ๊ฒฝ์ฐ ์ฌ์ฉํ  ์ ์์ต๋๋ค.
- ํนํ, `@types/react`์ `@types/react-dom`๊ฐ ์ค์น๋์ด ์๋์ง ํ์ธ์ด ํ์ํฉ๋๋ค. ([์ต์ํ์ง ์์ ๋ด์ฉ์ด๋ผ๋ฉด DefinitelyTyped project ์ ๋ํด ๋ ์์๋ณด์ธ์.](https://definitelytyped.org/))
- ๋ํ ๋ง์ React + TypeScript bolierplates๋ค์ด ์์ต๋๋ค. [์ฐ๋ฆฌ์ ๋ค๋ฅธ ๋ฆฌ์์ค ๋ฆฌ์คํธ](https://react-typescript-cheatsheet.netlify.app/docs/basic/recommended/resources/)๋ฅผ ํ์ธํด์ฃผ์ธ์.

</details>

#### ๋น๋์ค ํํ ๋ฆฌ์ผ

์๋์ 7๋ถ๋ก ๊ตฌ์ฑ๋ "React Typescript Course" ๋น๋์ค ์๋ฆฌ์ฆ๋ฅผ ํตํด TypeScript with React์ ๋ํ ์๊ฐ๋ฅผ ๋ค์ ์ ์์ต๋๋ค.

<a href="https://www.youtube.com/watch?v=PL1NUl7fQ2I&list=PLG-Mk4wQm9_LyKE5EwoZz2_GGXR-zJ5Ml">
    <img
        width="200px"
        alt="react typescript course video series"
        src="https://i.imgur.com/IIG0Xu9.jpeg"
    />
</a>

<!--END-SECTION:setup-->

### Section 2: ์์ํ๊ธฐ

<!--START-SECTION:function-components-->

#### ํจ์ ์ปดํฌ๋ํธ

ํจ์ ์ปดํฌ๋ํธ๋ `props`๋ฅผ ๋งค๊ฐ๋ณ์๋ก ๋ฐ๊ณ  JSX element๋ฅผ ๋ฐํํ๋ ์ผ๋ฐ์ ์ธ ํจ์๋ก ์์ฑ๋  ์ ์์ต๋๋ค.

```tsx
// props์ ํ์ ์ ์ - ๋ ๋ง์ ์์๋ "์ปดํฌ๋ํธ Props ํ์ดํ"์์ ํ์ธํ  ์ ์์ต๋๋ค.
type AppProps = {
  message: string;
}; /* export ํ๋ค๋ฉด consumer๊ฐ extendํ  ์ ์๋๋ก `interface`๋ฅผ ์ฌ์ฉํ์ธ์. */

// ํจ์ ์ปดํฌ๋ํธ๋ฅผ ์ ์ํ  ์ ์๋ ๊ฐ์ฅ ์ฌ์ด ๋ฐฉ๋ฒ; return type์ ์ถ๋ก ๋ฉ๋๋ค.
const App = ({ message }: AppProps) => <div>{message}</div>;

// ์ค์๋ก ๋ค๋ฅธ ํ์์ ๋ฐํํ์์ ๋ ์๋ฌ๊ฐ raise ๋๋๋ก return type์ ๋ช์ํ  ์ ์์ต๋๋ค.
const App = ({ message }: AppProps): JSX.Element => <div>{message}</div>;

// type ์ ์ธ์ ํจ์ ์ปดํฌ๋ํธ ์ ์ธ์ ํฌํจ์ํฌ ์ ์์ต๋๋ค.;์ด ๋ฐฉ๋ฒ์ prop types์ ์ด๋ฆ์ ๋ถ์ด์ง ์์๋ ๋์ง๋ง ์ฝ๋๊ฐ ๋ฐ๋ณต๋ฉ๋๋ค.
const App = ({ message }: { message: string }) => <div>{message}</div>;
```

> Tip: type destructure ์ ์ธ์ ์ํด [Paul Shen's VS Code Extension](https://marketplace.visualstudio.com/items?itemName=paulshen.paul-typescript-toolkit)๋ฅผ ์ฌ์ฉํ  ์๋ ์์ต๋๋ค. ([keyboard shortcut](https://twitter.com/_paulshen/status/1392915279466745857?s=20)์ ์ถ๊ฐ ํ์ธ์.)

<details>

<summary><b><code>React.FC</code>๊ฐ ๊ถ์ฅ๋์ง ์๋ ์ด์ ๋ ๋ฌด์์ผ๊น์? <code>React.FunctionComponent</code>/<code>React.VoidFunctionComponent</code>๋ ์ด๋ค๊ฐ์?</b></summary>

React+TypeScript codebases์์ ๋ค์ ๋ณด์์ ์ ์์ต๋๋ค.

```tsx
const App: React.FunctionComponent<{ message: string }> = ({ message }) => <div>{message}</div>;
```

ํ์ง๋ง, ํ์ฌ `React.FunctionComponent` (๋๋ ๊ฐ๋ตํ๊ฒ ์จ์ `React.FC`)๋ [๊ถ์ฅ๋์ง ์๋๋ค๋ ๊ฒ](https://github.com/facebook/create-react-app/pull/8177)์ ๋๋ถ๋ถ์ ์ฌ๋๋ค์ด ๋์ํฉ๋๋ค. ๋ฌผ๋ก  ์ด ์ฃผ์ ์ ๋ํ ๋ฏธ๋ฌํ ์๊ฒฌ ์ฐจ์ด๊ฐ ์์ ์๋ ์์ง๋ง, ๋ง์ฝ ์ด ์๊ฒฌ์ ๋์ํ๊ณ  `React.FC`๋ฅผ ๋น์ ์ ์ฝ๋๋ฒ ์ด์ค์์ ์ ๊ฑฐํ๊ณ  ์ถ๋ค๋ฉด, [์ด jscodeshift codemond](https://github.com/gndelia/codemod-replace-react-fc-typescript)๋ฅผ ์ฌ์ฉํ  ์ ์์ต๋๋ค.

"์ผ๋ฐ์ ์ธ ํจ์" ๋ฒ์ ๊ณผ์ ์ฐจ์ด์ ๋ค์ ๋ค์๊ณผ ๊ฐ์ต๋๋ค.

- `React.FunctionComponent`๋ return type์ ๋ช์์ ์ผ๋ก ๋ฐํ๋๋ค. ํ์ง๋ง ์ผ๋ฐ์ ์ธ ํจ์ ๋ฒ์ ์ ์์์ ์๋๋ค(๋๋ ์ถ๊ฐ์ ์ธ ์ด๋ธํ์ด์(annotation)์ด ํ์ํฉ๋๋ค).

- `displayName`, `propTypes`, ๊ทธ๋ฆฌ๊ณ  `defaultProps`์ ๊ฐ์ static properties๋ฅผ ์ํ ์๋์์ฑ(autocomplete)๊ณผ ํ์ ์ฒดํฌ(Typechecking)๋ฅผ ์ง์ํฉ๋๋ค.

  - `React.FunctionComponent`์ ํจ๊ป `defaultProps`์ ์ฌ์ฉํ๋๋ฐ ๋ช ๊ฐ์ง ์๋ ค์ง ๋ฌธ์ ๊ฐ ์์ต๋๋ค. [๋ฌธ์ ์ ๋ํ ์์ธํ ๋ด์ฉ](https://github.com/typescript-cheatsheets/react/issues/87)์ ํ์ธํ์ธ์. ์ฐ๋ฆฌ๋ ๊ฐ๋ฐ์๋์ด ์ฐพ์๋ณผ ์ ์๋ ๋ณ๊ฐ์ `defaultProps` ์น์์ ์ ๊ณตํ๊ณ  ์์ต๋๋ค.

- [React 18 type ์๋ฐ์ดํธ](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/56210) ์ด์ ์๋, `React.FunctionComponent`์ด `children`์ ๋ํ ์์์ ์ธ ์ ์(implicit definition)๋ฅผ ์ ๊ณตํ์์ต๋๋ค. ์ด๊ฒ์ ์ด๋ค ํ ๋ก  ๊ณผ์ ์ ๊ฑฐ์ณค๊ณ  ๊ฒฐ๊ณผ์ ์ผ๋ก [`React.FC`๊ฐ Create React App TypeScript template์์ ์ ๊ฑฐ](https://github.com/facebook/create-react-app/pull/8177)๋ ์ด์  ์ค ํ๋๊ฐ ๋์์ต๋๋ค.

```tsx
// React 18 types ์ด์ 
const Title: React.FunctionComponent<{ title: string }> = ({ children, title }) => (
  <div title={title}>{children}</div>
);
```

<details>
<summary>(Deprecated)<b><code>React.VoidFunctionComponent</code> ๋๋ <code>React.VFC</code> ์ฌ์ฉํ๊ธฐ</b></summary>

[@types/react 16.9.48](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/46643)์์, `React.VoidFunctionComponent` ๋๋ `React.VFC` type์ `children`์ ๋ช์์ ์ผ๋ก ํ์ดํ(typing) ํ๊ธฐ ์ํด ์ถ๊ฐ๋์์ต๋๋ค.
ํ์ง๋ง, `React.VFC`์ `React.VoidFunctionComponent`๋ React 18 (https://github.com/DefinitelyTyped/DefinitelyTyped/pull/59882) ์์ ๋์ด์ ์ฌ์ฉ๋์ง ์๊ฒ ๋์์ต๋๋ค(deprecated). ๋ฐ๋ผ์ ์ด ์์๋ฐฉํธ์ React 18+ ์์ ๋์ด์ ๊ถ์ฅ๋์ง ์์ต๋๋ค.

์ผ๋ฐ์ ์ธ ํจ์ ์ปดํฌ๋ํธ๋ `React.FC`๋ฅผ ์ฌ์ฉํด ์ฃผ์ธ์.

```ts
type Props = { foo: string };

// ์ง๊ธ์ ๊ด์ฐฎ์ง๋ง, ๋ฏธ๋์๋ ์๋ฌ๋ฅผ ๋ฐ์์ํฌ ๊ฒ์๋๋ค.
const FunctionComponent: React.FunctionComponent<Props> = ({ foo, children }: Props) => {
  return (
    <div>
      {foo} {children}
    </div>
  ); // OK
};

// ์ง๊ธ์ ์๋ฌ๋ฅผ ๋ฐ์์ํค๊ณ , ๋ฏธ๋์๋ ๋์ด์ ์ฌ์ฉ๋์ง ์์๊ฒ์๋๋ค.(Deprecated)
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

- _๋ฏธ๋์๋_, props๋ฅผ ์๋์ผ๋ก `readonly` ๋ผ๊ณ  ํ์ํ  ์๋ ์์ต๋๋ค. ํ์ง๋ง, props ๊ฐ์ฒด๊ฐ ํ๋ผ๋ฏธํฐ ๋ฆฌ์คํธ์์ destructure ๋๋ค๋ฉด, ์ด๊ฒ์ ์๋ฏธ์๋ ํ๋ ์๋๋ค.

๋๋ถ๋ถ์ ๊ฒฝ์ฐ์๋ ์ด๋ค syntax๋ฅผ ์ฌ์ฉํ๋์ง ํฐ ์ฐจ์ด๊ฐ ์์ง๋ง, `React.FunctionComponent`์ ๋ณด๋ค ๋ช์์ ์ธ ํน์ฑ์ ์ ํธํ๋ ๊ฒ์ด ์ข์๊ฒ์๋๋ค.

</details>

<details>
<summary><b>์ฃผ์ํด์ผ ํ  ์ฌํญ</b></summary>

๋ค์์ ํจํด์ ์ง์๋์ง ์์ต๋๋ค. :

**์กฐ๊ฑด๋ถ ๋ ๋๋ง(conditional rendering)**

```tsx
const MyConditionalComponent = ({ shouldRender = false }) => (shouldRender ? <div /> : false); // JS ์์๋ ์ด๋ ๊ฒ ํ์ง ๋ง์ญ์์ค.
const el = <MyConditionalComponent />; // ์๋ฌ๋ฅผ throw ํฉ๋๋ค.
```

์ด ํจํด์ด ์ง์๋์ง ์๋ ์ด์ ๋ ์ปดํ์ผ๋ฌ์ ํ๊ณ ๋๋ฌธ์๋๋ค. ํจ์ ์ปดํฌ๋ํธ๋ JSX expression ๋๋ `null` ์ด์ธ์ ๋ค๋ฅธ ์ด๋ค ๊ฒ๋ ๋ฐํํ  ์ ์์ต๋๋ค. ๋ฐํํ  ์ ์๋ ๊ฒ์ด ๋ฐํ๋๋ค๋ฉด ํด๋น ํ์์ `Element`์ ํ ๋น๋  ์ ์๋ค๋ ์๋ฌ ๋ฉ์ธ์ง๋ฅผ ๋ณด๊ฒ๋  ๊ฒ์๋๋ค. ("{the other type} is not assignable to `Element`.")

**Array.fill**

```tsx
const MyArrayComponent = () => Array(5).fill(<div />);
const el2 = <MyArrayComponent />; // throws an error
```

์์ฝ๊ฒ๋ ํจ์์ ํ์์ annotate ํ๋ ๊ฒ์ ์๋ฌด๋ฐ ๋์์ด ๋์ง ์์๊ฒ์๋๋ค. React๊ฐ ์ง์ํ๋ ๋ค๋ฅธ ํน๋ณํ ํ์(exotic type)์ ๋ฐํํ๊ณ ์ ํ๋ค๋ฉด ํ์ ํ๋ช(type assertion)์ ์ํํด์ผ ํฉ๋๋ค. :

```tsx
const MyArrayComponent = () => Array(5).fill(<div />) as any as JSX.Element;
```

[์ฌ๊ธฐ์ @ferdaber ์ ์ค๋ช์ ํ์ธํด๋ณด์ธ์](https://github.com/typescript-cheatsheets/react/issues/57).

</details>

<!--END-SECTION:function-components-->

<!--START-SECTION:hooks-->

#### Hooks

Hook์ [`@types/react` v16.8 ์ด์๋ถํฐ ์ง์๋ฉ๋๋ค](https://github.com/DefinitelyTyped/DefinitelyTyped/blob/a05cc538a42243c632f054e42eab483ebf1560ab/types/react/index.d.ts#L800-L1031).

#### useState

ํ์ ์ถ๋ก (Type inference)์ ๊ฐ๋จํ ๊ฐ๋ค์ ์ ์๋ํฉ๋๋ค:

```tsx
const [state, setState] = useState(false);
// `state` ๋ boolean ์ผ๋ก ์ถ๋ก ๋ฉ๋๋ค.
// `setState` ๋ boolean ๊ฐ ๋ง์ ๋ฐ์ต๋๋ค.
```

ํ์ ์ถ๋ก ์ ๋ณต์กํ ํ์์ ์ฌ์ฉํด์ผ ํ๋ค๋ฉด [์ถ๋ก ๋ ํ์(Inferred Types) ์ฌ์ฉํ๊ธฐ](https://react-typescript-cheatsheet.netlify.app/docs/basic/troubleshooting/types/#using-inferred-types) ๋ ํ์ธํด๋ณด์ธ์.

ํ์ง๋ง ๋ง์ hook ๋ค์ null ๊ฐ์ ๊ฐ๋ฅผ ๋ํดํธ ๊ฐ์ผ๋ก ์ด๊ธฐํ ํ๊ธฐ ๋๋ฌธ์ ์ด๋ป๊ฒ ํ์์ ์ง์ ํ๋์ง ๊ถ๊ธํ  ์ ์์ต๋๋ค. ๋ช์์ ์ผ๋ก ํ์์ ์ ์ธํ๊ณ , union type์ ์ฌ์ฉํ์ธ์.:

```tsx
const [user, setUser] = useState<User | null>(null);

// later...
setUser(newUser);
```

๋ง์ฝ useState์ค์  ์งํ์ state๊ฐ ์ด๊ธฐํ๋๊ณ  ๊ทธ ์ดํ์ ํญ์ ๊ฐ์ ๊ฐ์ง๋ค๋ฉด, ํ์ ํ๋ช(type assertions)์ ์ฌ์ฉํ  ์๋ ์์ต๋๋ค.

```tsx
const [user, setUser] = useState<User>({} as User);

// later...
setUser(newUser);
```

์ด ๋ฐฉ๋ฒ์ ์ผ์์ ์ผ๋ก ํ์์คํฌ๋ฆฝํธ ์ปดํ์ผ๋ฌ์๊ฒ `{}`๊ฐ `User`์ type์ด๋ผ๊ณ  "๊ฑฐ์ง๋ง" ํฉ๋๋ค. ๊ทธ ํ์ `user` state๋ฅผ ์ค์ ํ์ฌ์ผ ํฉ๋๋ค. ๊ทธ๋ ์ง ์์ผ๋ฉด ๋๋จธ์ง ์ฝ๋๊ฐ `user`๋ `User` ํ์์ด๋ผ๋ ์ฌ์ค์ ์์กด๊ณ  ์ด๊ฒ์ ๋ฐํ์ ์๋ฌ๋ก ์ด์ด์ง ์ ์์ต๋๋ค.

#### useReducer

Reducer actions๋ฅผ ์ํด [Discriminated Unions](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes-func.html#discriminated-unions)๋ฅผ ์ฌ์ฉํ  ์ ์์ต๋๋ค. reducer์ return type์ ์ ์ํ๋ ๊ฒ์ ์์ง ๋ง์ธ์. ๊ทธ๋ ์ง ์์ผ๋ฉด ํ์์คํฌ๋ฆฝํธ๊ฐ return type์ ์ถ๋ก ํ  ๊ฒ์๋๋ค.

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

[TypeScript Playground์์ ๋ณด๊ธฐ](https://www.typescriptlang.org/play?#code/LAKFEsFsAcHsCcAuACAVMghgZ2QJQKYYDGKAZvLJMgOTyEnUDcooRsAdliuO+IuBgA2AZUQZE+ZAF5kAbzYBXdogBcyAAwBfZmBCIAntEkBBAMIAVAJIB5AHLmAmgAUAotOShkyAD5zkBozVqHiI6SHxlagAaZGgMfUFYDAATNXYFSAAjfHhNDxAvX1l-Q3wg5PxQ-HDImLiEpNTkLngeAHM8ll1SJRJwDmQ6ZIUiHIAKLnEykqNYUmQePgERMQkY4n4ONTMrO0dXAEo5T2aAdz4iAAtkMY3+9gA6APwj2ROvImxJYPYqmsRqCp3l5BvhEAp4Ow5IplGpJhIHjCUABqTB9DgPeqJFLaYGfLDfCp-CIAoEFEFeOjgyHQ2BKVTNVb4RF05TIAC0yFsGWy8Fu6MeWMaB1x5K8FVIGAUglUwK8iEuFFOyHY+GVLngFD5Bx0Xk0oH13V6myhplZEm1x3JbE4KAA2vD8DFkuAsHFEFcALruAgbB4KAkEYajPlDEY5GKLfhCURTHUnKkQqFjYEAHgAfHLkGb6WpZI6WfTDRSvKnMgpEIgBhxTIJwEQANZSWRjI5SdPIF1u8RXMayZ7lSphEnRWLxbFNagAVmomhF6fZqYA9OXKxxM2KQWWK1WoTW643m63pB2u+7e-3SkEQsPamOGik1FO55p08jl6vdxuKcvv8h4yAmhAA)

<details>

<summary><b><code>Redux</code>์์ <code>Reducer</code>์ ํจ๊ป ์ฌ์ฉํ๊ธฐ</b></summary>

Reducer funciton์ ์์ฑํ๊ธฐ ์ํด [redux](https://github.com/reduxjs/redux)๋ฅผ ์ฌ์ฉํ๋ ๊ฒฝ์ฐ, return type์ ์ฒ๋ฆฌํ๋ `Reducer<State, Action>` ํ์์ ํธ๋ฆฌํ helper๋ฅผ ์ฌ์ฉํ  ์ ์์ต๋๋ค.

์์ reducer example์ ๋ค์๊ณผ ๊ฐ์ด ๋ฐ๋ ์ ์์ต๋๋ค. :

```tsx
import { Reducer } from 'redux';

export function reducer: Reducer<AppState, Action>() {}
```

</details>

#### useEffect / useLayoutEffect

`userEffect`์ `userLayoutEffect` ๋ ๋ค <b>side effect</b>๋ฅผ ์ํํ๊ธฐ ์ํด ์ฌ์ฉ๋๊ณ  ์ ํ์ ์ผ๋ก cleanup function์ ๋ฐํํฉ๋๋ค. ์ด๊ฒ์ ๋ง์ฝ ์ด hook๋ค์ด ๋ฐํ ๊ฐ์ ์ฒ๋ฆฌํ์ง ์๋๋ค๋ฉด, type์ด ํ์ ์๋ค๋ ๋ป์๋๋ค. `useEffect`๋ฅผ ์ฌ์ฉํ  ๋, ํจ์ ๋๋ `undefined` ์ด์ธ์ ๋ค๋ฅธ ๊ฒ์ ๋ฐํํ์ง ์๋๋ก ์ฃผ์ํ์ธ์. ๊ทธ๋ ์ง ์์ผ๋ฉด TypeScript์ React๋ ๋น์ ์๊ฒ ๋น๋ช์ ์ง๋ฅผ๊ฒ์๋๋ค. Arros functions๋ฅผ ์ฌ์ฉํ๋ค๋ฉด ์ด ๋ฌธ์ ๋ ๋ค์ ํ์ํ๊ธฐ ์ด๋ ค์ธ ์ ์์ต๋๋ค. :

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
  // ๋์ ์์! setTimeout์ ์๋ฌต์ ์ผ๋ก ์ซ์๋ฅผ ๋ฐํํ๊ณ  ์์ต๋๋ค.
  // arrow function์ body๊ฐ ์ค๊ดํธ๋ก ๊ฐ์ธ์ง์ง ์์๊ธฐ ๋๋ฌธ์๋๋ค.
  return null;
}
```

<details>
<summary><b>์ ์์์ ๋ํ ํด๊ฒฐ์ฑ</b></summary>

```tsx
function DelayedEffect(props: { timerMs: number }) {
  const { timerMs } = props;

  useEffect(() => {
    setTimeout(() => {
      /* do stuff */
    }, timerMs);
  }, [timerMs]);
  // ๋ ๋์ ๋ฐฉ๋ฒ; ํ์คํ๊ฒ undefined๋ฅผ ๋ฐํํ๊ธฐ ์ํด์ void keyword๋ฅผ ์ฌ์ฉํ์ธ์.
  return null;
}
```

</details>

#### useRef

TypeScript์์ `useRef`๋ type argument๊ฐ ์ด๊ธฐ ๊ฐ์ ์์ ํ ํฌํจ(cover)ํ๋์ง ์๋์ง์ ๋ฐ๋ผ[read-only](https://github.com/DefinitelyTyped/DefinitelyTyped/blob/abd69803c1b710db58d511f4544ec1b70bc9077c/types/react/v16/index.d.ts#L1025-L1039)๋๋ [mutable](https://github.com/DefinitelyTyped/DefinitelyTyped/blob/abd69803c1b710db58d511f4544ec1b70bc9077c/types/react/v16/index.d.ts#L1012-L1023) ๋ ์ค ํ๋๋ฅผ ๋ฐํํฉ๋๋ค. ๊ฐ์์ use case์ ๋ง๋ ๊ฒ์ ์ ํํ์ธ์.

##### Option 1: DOM element ref

**[DOM element์ ์ ๊ทผํ๊ธฐ ์ํด์๋](https://reactjs.org/docs/refs-and-the-dom.html):** element type ๋ง์ argument๋ก ๋๊ฒจ์ฃผ๊ณ  `null`์ ์ด๊ธฐ ๊ฐ์ผ๋ก ์ฌ์ฉํ์ธ์. ์ด ๊ฒฝ์ฐ์, ๋ฐํ๋๋ reference๋ React์ ์ํด ๊ด๋ฆฌ๋๋ read-only `.current`๋ฅผ ๊ฐ์ง ๊ฒ์๋๋ค. TypeScript๋ ์ด ref๋ฅผ element์ `ref` prop์ผ๋ก ์ ๋ฌ ๋ฐ๊ธฐ๋ฅผ ๊ธฐ๋ํฉ๋๋ค. :

```tsx
function Foo() {
  // - ๊ฐ๋ฅํ ์์ธํ๊ฒ ์์ฑํ์ธ์. ์๋ฅผ๋ค๋ฉด, HTMLDivElement๋ HTMLElement๋ณด๋ค ๋ ์ข๊ณ ,
  // Element๋ณด๋ค๋ ํจ์  ๋ ์ข์ ์ ํ์๋๋ค.
  // - ๊ธฐ์ ์ ์ผ๋ก ๋งํ์๋ฉด, ์ด๊ฒ์ RefObject<HTMLDivElement>๋ฅผ ๋ฐํํฉ๋๋ค.
  const divRef = useRef<HTMLDivElement>(null);

  useEffect(() => {
    // ref.current๊ฐ null์ผ ์ ์๋ค๋ ๊ฒ์ ์ฃผ์ํ์ธ์.
    // ์ด๊ฒ์ ๋น์ ์ด ์กฐ๊ฑด์ ๋ฐ๋ผ์ ref๋(ref-ed) element๋ฅผ renderํ๊ฑฐ๋
    // ํ ๋นํ๋ ๊ฒ์ ์์ ์ ์๊ธฐ ๋๋ฌธ์ ์์ธกํ  ์ ์๋ ํ์์๋๋ค.
    if (!divRef.current) throw Error("divRef is not assigned");

    // ์ด์  divRef.current๋ ํ์คํ๊ฒ HTMLDivElement ์๋๋ค.
    doSomethingWith(divRef.current);
  });

  // React๊ฐ ๋น์ ์ ์ํด ref๋ฅผ ๊ด๋ฆฌํ  ์์๋๋ก element์๊ฒ ref๋ฅผ ์ ๋ฌํด ์ฃผ์ธ์.
  return <div ref={divRef}>etc</div>;
}
```

๋ง์ฝ `divRef.current`๊ฐ ์ ๋๋ก null์ด ์๋๊ฒ์ด๋ผ๋ ๊ฒ์ ํ์ ํ๋ค๋ฉด, non-null assertion operator `!`์ ์ฌ์ฉํ๋ ๊ฒ๋ ๊ฐ๋ฅํฉ๋๋ค. :

```tsx
const divRef = useRef<HTMLDivElement>(null!);
// ๋์ค์... ์ด๊ฒ์ด null ์ธ์ง ํ์ธํ  ํ์๊ฐ ์์ต๋๋ค.
doSomethingWith(divRef.current);
```

๋น์ ์ด type safety๊ฐ ๋ณด์ฅ๋๋ค๊ณ  ๋ฏธ๋ฆฌ ๊ฐ์ ํ๊ณ  ์ฝ๋๋ฅผ ์์ฑํ๋ค๋ ๊ฒ์ ์ฃผ์ํด์ผ ํฉ๋๋ค. ๋ ๋๋ง ๊ณผ์ ์์ ref๋ฅผ element์ ํ ๋นํ๋ ๊ฒ์ ์๊ฑฐ๋, ref๋(ref-ed) element๊ฐ ์กฐ๊ฑด๋ถ ๋ ๋๋ง ๋๋ค๋ฉด runtime error๊ฐ ๋ฐ์ํ  ๊ฒ์๋๋ค.

<details>
<summary><b>Tip: ์ด๋ค <code>HTMLElement</code>๋ฅผ ์ฌ์ฉํ ์ง ์ ํํ๊ธฐ</b></summary>
  
Ref๋ ๋ช์์ฑ(specificity)์ ํ์๋ก ํฉ๋๋ค. ์ฆ, `HTMLElement` ๋ง์ ๋ช์ํ๋ ๊ฒ์ ์ถฉ๋ถํ์ง ์๋ค๋ ๋ง์๋๋ค. ๋ง์ฝ ๋น์ ์ด ํ์ํ element type์ ์ด๋ฆ์ ๋ชจ๋ฅธ๋ค๋ฉด, [lib.dom.ts](https://github.com/microsoft/TypeScript/blob/v3.9.5/lib/lib.dom.d.ts#L19224-L19343)์์ ํ์ธํ๊ฑฐ๋ ์๋์ ์ผ๋ก type error๋ฅผ ๋ฐ์์ํค๊ณ  language service๊ฐ type์ ์ด๋ฆ์ ์๋ ค์ฃผ๋๋ก ํ  ์ ์์ต๋๋ค.

![image](https://user-images.githubusercontent.com/6764957/116914284-1c436380-ac7d-11eb-9150-f52c571c5f07.png)

</details>

##### Option 2: Mutable value ref

**[mutable value๋ฅผ ๊ฐ์ง๊ธฐ ์ํด์๋](https://reactjs.org/docs/hooks-faq.html#is-there-something-like-instance-variables):** ์ํ๋ type์ ์ฌ์ฉํ๊ณ  ์ด๊ธฐ ๊ฐ์ด ์์ ํ ํด๋น type์ ์ํ๋์ง ํ์ธํ์ธ์.

```tsx
function Foo() {
  // ๊ธฐ์ ์ ์ผ๋ก ๋งํ์๋ฉด, ์ด๊ฒ์ MutableRefObject<number | null>์ ๋ฐํํฉ๋๋ค.
  const intervalRef = useRef<number | null>(null);

  // ๋น์ ์ด ์ง์  ref๋ฅผ ๊ด๋ฆฌํฉ๋๋ค. (์ด๊ฒ์ด MutableRefObject๋ผ๊ณ  ๋ถ๋ฆฌ๋ ์ด์ ์ด์ฃ .)
  useEffect(() => {
    intervalRef.current = setInterval(...);
    return () => clearInterval(intervalRef.current);
  }, []);

  // ref๋ element์ "ref" prop์ผ๋ก ์ ๋ฌ๋์ง ์์ต๋๋ค.
  return <button onClick={/* clearInterval the ref */}>Cancel timer</button>;
}
```

##### ๋ค์์ ์๋ฃ๋ ํ์ธํด ๋ณด์ธ์.

- [@rajivpunjabi๊ฐ ์์ฑํ ๊ด๋ จ ์ด์](https://github.com/typescript-cheatsheets/react/issues/388) - [Playground](https://www.typescriptlang.org/play#code/JYWwDg9gTgLgBAKjgQwM5wEoFNkGN4BmUEIcARFDvmQNwCwAUI7hAHarwCCYYcAvHAAUASn4A+OAG9GjOHAD0CBLLnKGcxHABiwKBzgQwMYGxS4WUACbBWAczgwIcSxFwBXEFlYxkxtgDoVTQBJVmBjZAAbOAA3KLcsOAB3YEjogCNE1jc0-zgAGQBPG3tHOAAVQrAsAGVcKGAjOHTCuDdUErhWNgBabLSUVFQsWBNWA2qoX2hA9VU4AGFKXyx0AFk3H3TIxOwCOAB5dIArLHwgpHcoSm84MGJJmFbgdG74ZcsDVkjC2Y01f7yFQsdjvLAEACM-EwVBg-naWD2AB4ABLlNb5GpgZCsACiO083jEgn6kQAhMJ6HMQfpKJCFpE2IkBNg8HCEci0RisTj8VhCTBiaSKVSVIoAaoLnBQuFgFFYvFEikBpkujkMps4FgAB7VfCdLmY7F4gleOFwAByEHg7U63VYfXVg2Go1MhhG0ygf3mAHVUtF6jgYLtwUdTvguta4Bstjs9mGznCpVcbvB7u7YM90B8vj9vYgLkDqWxaeCAEzQ1n4eHDTnoo2801EknqykyObii5SmpnNifA5GMZmCzWOwOJwudwC3xjKUyiLROKRBLJf3NLJO9KanV64xj0koVifQ08k38s1Sv0DJZBxIx5DbRGhk6J5Nua5mu4PEZPOAvSNgsgnxsHmXZzIgRZyDSYIEAAzJWsI1k+BCovWp58gKcAAD5qmkQqtqKHbyCexoYRecw7IQugcAs76ptCdIQv4KZmoRcjyMRaGkU28A4aSKiUXAwwgpYtEfrcAh0mWzF0ax7bsZx3Lceetx8eqAlYPAMAABa6KJskSXAdKwTJ4kwGxCjyKy-bfK05SrDA8mWVagHAbZeScOY0CjqUE6uOgqDaRAOSfKqOYgb8KiMaZ9GSeCEIMkyMVyUwRHWYc7nSvAgUQEk6AjMQXpReWyWGdFLHeBZHEuTCQEZT8xVwaV8BxZCzUWZQMDvuMghBHASJVnCWhTLYApiH1chIqgxpGeCfCSIxAC+Yj3o+8YvvgSLyNNOLjeBGhTTNdLzVJy3reGMBbTtrB7RoB3XbNBAneCsHLatcbPhdV3GrdB1WYhw3IKNZq-W2DCLYRO7QPAljgsgORcDwVJAA)
- [Stefan Baumgartner์ ์์](https://fettblog.eu/typescript-react/hooks/#useref) - [Playground](https://www.typescriptlang.org/play/?jsx=2#code/JYWwDg9gTgLgBAJQKYEMDG8BmUIjgIilQ3wFgAoCzAVwDsNgJa4AVJADxgElaxqYA6sBgALAGIQ01AM4AhfjCYAKAJRwA3hThwA9DrjBaw4CgA2waUjgB3YSLi1qp0wBo4AI35wYSZ6wCeYEgAymhQwGDw1lYoRHCmEBAA1oYA5nCY0HAozAASLACyADI8fDAAoqZIIEi0MFpwaEzS8IZllXAAvIjEMAB0MkjImAA8+cWl-JXVtTAAfEqOzioA3A1NtC1wTPIwirQAwuZoSV1wql1zGg3aenAt4RgOTqaNIkgn0g5ISAAmcDJvBA3h9TsBMAZeFNXjl-lIoEQ6nAOBZ+jddPpPPAmGgrPDEfAUS1pG5hAYvhAITBAlZxiUoRUqjU6m5RIDhOi7iIUF9RFYaqIIP9MlJpABCOCAUHJ0eDzm1oXAAGSKyHtUx9fGzNSacjaPWq6Ea6gI2Z9EUyVRrXV6gC+DRtVu0RBgxuYSnRIzm6O06h0ACpIdlfr9jExSQyOkxTP5GjkPFZBv9bKIDYSmbNpH04ABNFD+CV+nR2636kby+BETCddTlyo27w0zr4HycfC6L0lvUjLH7baHY5Jas7BRMI7AE42uYSUXed6pkY6HtMDulnQruCrCg2oA)

#### useImperativeHandle

ํด๋น [Stackoverflow answer](https://stackoverflow.com/a/69292925/5415299)์ ๋ฐ๋ฅด๋ฉด ๋ค์๊ณผ ๊ฐ์ต๋๋ค.:

```tsx
// Countdown.tsx

// forwardRef๋ก ์ ๋ฌ๋  handle type์ ์ ์ํฉ๋๋ค
export type CountdownHandle = {
  start: () => void;
};

type CountdownProps = {};

const Countdown = forwardRef<CountdownHandle, CountdownProps>((props, ref) => {
  useImperativeHandle(ref, () => ({
    // start() ๋ ์ฌ๊ธฐ์ ํ์ ์ถ๋ก (type inference) ๋ฉ๋๋ค
    start() {
      alert("Start");
    },
  }));

  return <div>Countdown</div>;
});
```

```tsx
// ์ด ์ปดํฌ๋ํธ๋ Countdown ์ปดํฌ๋ํธ๋ฅผ ์ฌ์ฉํฉ๋๋ค

import Countdown, { CountdownHandle } from "./Countdown.tsx";

function App() {
  const countdownEl = useRef<CountdownHandle>(null);

  useEffect(() => {
    if (countdownEl.current) {
      // start()๋ ์ฌ๊ธฐ์๋ ํ์ ์ถ๋ก (type inference) ๋ฉ๋๋ค.
      countdownEl.current.start();
    }
  }, []);

  return <Countdown ref={countdownEl} />;
}
```

##### ๋ค์์ ์๋ฃ๋ ํ์ธํด๋ณด์ธ์:

- [ForwardRefRenderFunction ์ฌ์ฉํ๊ธฐ](https://stackoverflow.com/a/62258685/5415299)

#### Custom Hooks

๋ง์ฝ Custom Hook์์ array๋ฅผ returnํ๋ค๋ฉด, array์ ๊ฐ ์์น์์ ๊ฐ๊ธฐ ๋ค๋ฅธ type์ ๊ฐ์ง๊ธฐ๋ฅผ ์ํ๊ฒ ์ง๋ง TypeScript๋ union type์ผ๋ก ์ถ๋ก ํ  ๊ฒ์ด๊ธฐ ๋๋ฌธ์ ํ์ ์ถ๋ก ์ ํผํ๊ณ  ์ถ์ ๊ฒ์๋๋ค. ์ด๋ฌํ ์ํฉ์์ [TS 3.4 const assertions](https://devblogs.microsoft.com/typescript/announcing-typescript-3-4/#const-assertions)์ ์ฌ์ฉํ  ์ ์์ต๋๋ค.

```tsx
import { useState } from "react";

export function useLoading() {
  const [isLoading, setState] = useState(false);
  const load = (aPromise: Promise<any>) => {
    setState(true);
    return aPromise.finally(() => setState(false));
  };
  return [isLoading, load] as const; // (boolean | typeof load)[]์ด ์๋ [boolean, typeof load]์ผ๋ก ์ถ๋ก ํฉ๋๋ค.
}
```

[TypeScript Playground์์ ํ์ธํด ๋ณด๊ธฐ](https://www.typescriptlang.org/play/?target=5&jsx=2#code/JYWwDg9gTgLgBAJQKYEMDG8BmUIjgcilQ3wFgAoCpAD0ljkwFcA7DYCZuRgZyQBkIKACbBmAcwAUASjgBvCnDhoO3eAG1g3AcNFiANHF4wAyjBQwkAXTgBeRMRgA6HklPmkEzCgA2vKQG4FJRV4b0EhWzgJFAAFHBBNJAAuODjcRIAeFGYATwA+GRs8uSDFIzcLCRgoRiQA0rgiGEYoTlj4xMdMUR9vHIlpW2Lys0qvXzr68kUAX0DpxqRm1rgNLXDdAzDhaxRuYOZVfzgAehO4UUwkKH21ACMICG9UZgMYHLAkCEw4baFrUSqVARb5RB5PF5wAA+cHen1BfykaksFBmQA)

์ด๋ฐ ๋ฐฉ๋ฒ์ผ๋ก, destructureํ์ ๋ destructuregํ ์์น์ ๋ฐ๋ผ ์ฌ๋ฐ๋ฅธ type์ ์ป์ ์ ์์ต๋๋ค.

<details>
<summary><b>๋์: tuple return type์ ํ๋ชํ๊ธฐ(assert)</b></summary>

๋ง์ฝ [const assertions์ด ์ฌ์ฉํ๊ธฐ ์ด๋ ต๋ค๋ฉด](https://github.com/babel/babel/issues/9800), ํจ์ return type์ ํ๋ช(assert)ํ๊ฑฐ๋ ์ ์ํ  ์ ์์ต๋๋ค.

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

๋ง์ custom hooks์ ์์ฑํ๋ค๋ฉด, ์๋์ผ๋ก tuples์ ํ์์ ๋ช์ํด์ฃผ๋ helper๋ ํฐ ๋์์ด ๋  ์ ์์ต๋๋ค.

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

ํ์ง๋ง React team์ ๋๊ฐ ์ด์์ ๊ฐ์ returnํ๋ custom hook์ tuple ๋์  ์ ์ ํ object๋ฅผ ์ฌ์ฉํ๋ ๊ฒ์ ๊ถ์ฅํ๋ค๋ ๊ฒ์ ์ฃผ์ํ์ธ์.

#### ๋ ๋ง์ Hooks + TypeScript ์ ๊ดํ ์ฝ์ ๊ฑฐ๋ฆฌ:

- https://medium.com/@jrwebdev/react-hooks-in-typescript-88fce7001d0d
- https://fettblog.eu/typescript-react/hooks/#useref

๋ง์ฝ React Hooks library๋ฅผ ์์ฑํ๊ณ  ์๋ค๋ฉด, ์ฌ์ฉ์๋ค์ด ์ฌ์ฉํ  ์ ์๋๋ก types๋ฅผ export ํด์ผ ํ๋ค๋ ๊ฒ์ ์์ง ๋ง์ธ์.

#### React Hooks + TypeScript Libraries ์์:

- https://github.com/mweststrate/use-st8
- https://github.com/palmerhq/the-platform
- https://github.com/sw-yx/hooks

[์ถ๊ฐํ  ๋ด์ฉ์ด ์๋์? issue๋ฅผ ์ฅ์ฑํ์ธ์!](https://github.com/typescript-cheatsheets/react/issues/new).

<!--END-SECTION:hooks-->

<!--START-SECTION:class-components-->

#### Class Components

TypeScript์์ `React.Component`๋ generic type (aka `React.Component<PropType, StateType>`)์๋๋ค. ๋ฐ๋ผ์ `React.Component`์ prop๊ณผ state type parameter๋ฅผ ์ ๋ฌํด์ผ ํฉ๋๋ค. :

```tsx
type MyProps = {
  // `interface`๋ฅผ ์ฌ์ฉํ๋ ๊ฒ๋ ๊ด์ฐฎ์ต๋๋ค
  message: string;
};
type MyState = {
  count: number; // ์ด๋ฐ ์์ผ๋ก
};
class App extends React.Component<MyProps, MyState> {
  state: MyState = {
    // ๋ ๋์ ํ์ ์ถ๋ก ์ ์ํด ์ ํ์ ์ผ๋ก ์์ฑํ ๋ ๋ฒ์งธ annotation
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

[TypeScript Playground ํ์ธํด ๋ณด๊ธฐ](https://www.typescriptlang.org/play/?jsx=2#code/JYWwDg9gTgLgBAJQKYEMDG8BmUIjgcilQ3wFgAoCmATzCTgFlqAFHMAZzgF44BvCuHAD0QuAFd2wAHYBzOAANpMJFEzok8uME4oANuwhwIAawFwQSduxQykALjjsYUaTIDcFAL4fyNOo2oAZRgUZW4+MzQIMSkYBykxEAAjFTdhUV1gY3oYAAttLx80XRQrOABBMDA4JAAPZSkAE05kdBgAOgBhXEgpJFiAHiZWCA4AGgDg0KQAPgjyQSdphyYpsJ5+BcF0ozAYYAgpPUckKKa4FCkpCBD9w7hMaDgUmGUoOD96aUwVfrQkMyCKIxOJwAAMZm8ZiITRUAAoAJTzbZwIgwMRQKRwOGA7YDRrAABuM1xKN4eW07TAbHY7QsVhsSE8fAptKWynawNinlJcAGQgJxNxCJ8gh55E8QA)

์ฌ์ฌ์ฉํ๊ธฐ ์ํด ์ด๋ฌํ types/interfaces๋ฅผ export/import/extend ํ  ์ ์๋ค๋ ๊ฒ์ ์์ง ๋ง์ธ์.

<details>
<summary><b>์ <code>state</code>๋ฅผ ๋ ๋ฒ annotate ํ ๊น์?</b></summary>

๋ฐ๋์ `state` class property์ annotateํ  ํ์๋ ์์ง๋ง, ์ด๋ ๊ฒ ํ๋ฉด `this.state`์ ์ ๊ทผํ๊ฑฐ๋ state๋ฅผ ์ด๊ธฐํ ํ  ๋ ๋ ๋์ ํ์ ์ถ๋ก ์ ๊ฐ๋ฅํ๊ฒ ํฉ๋๋ค.

๊ทธ ์ด์ ๋ ๋ ๊ฐ์ annotation์ ์๋ก ๋ค๋ฅธ ๋ฐฉ์์ผ๋ก ๋์ํ๊ธฐ ๋๋ฌธ์๋๋ค. ๋ ๋ฒ์งธ generic type parameter๋ `this.setState()`๊ฐ ์ฌ๋ฐ๋ฅด๊ฒ ๋์ํ๋๋ก ํด์ค๋๋ค. ์๋ํ๋ฉด ์ด ๋ฉ์๋๋ base class์์ ์ค๊ธฐ ๋๋ฌธ์๋๋ค. ํ์ง๋ง ์ปดํฌ๋ํธ ๋ด์์ `state`๋ฅผ ์ด๊ธฐํ ํ๋ ๊ฒ์ base implementation์ overrideํ๊ธฐ ๋๋ฌธ์ ์ปดํ์ผ๋ฌ์๊ฒ ์ฌ์ค์ ๋ค๋ฅธ ์์์ ํ๊ณ  ์์ง ์๋ค๋ ๊ฒ์ ์๋ ค์ค์ผ ํฉ๋๋ค. (=์ปดํ์ผ๋ฌ์๊ฒ ์ฌ์ค์ ๊ฐ์ ์์์ ํ๊ณ  ์๋ค๋ ๊ฒ์ ์๋ ค์ค์ผ ํฉ๋๋ค.)

[์ฌ๊ธฐ์ @ferdaber์ ์๊ฒฌ์ ํ์ธํด๋ณด์ธ์](https://github.com/typescript-cheatsheets/react/issues/57).

</details>

<details>
  <summary><b><code>readonly</code>๋ ํ์ ์๋ค</b></summary>

์ข์ข ์ํ ์ฝ๋์ props์ state๊ฐ ๋ณํ  ์ ์๋ค๊ณ  ํ์ํ๊ธฐ ์ํด `readonly`๋ฅผ ํฌํฉํ๋ ๊ฒ์ ๋ณผ ์ ์์ต๋๋ค.

```tsx
type MyProps = {
  readonly message: string;
};
type MyState = {
  readonly count: number;
};
```

`React.Component<P,S>`๊ฐ ์ด๋ฏธ props์ state๊ฐ ๋ณํ  ์ ์๋ค๊ณ  ํ์ํ๊ธฐ ๋๋ฌธ์ ์ถ๊ฐ์ ์ผ๋ก readonlyํ์๋ฅผ ํ  ํ์๊ฐ ์์ต๋๋ค. ([PR ๊ณผ discussion์ ํ์ธํ์ธ์!](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/26813))

</details>

**Class Methods**: ์๋ ํ๋๋ฐ๋ก ํ๋, ๋น์ ์ ํจ์๋ฅผ ์ํ ๋ชจ๋  arguments๋ type์ด ์์ด์ผ ํ๋ค๋ ๊ฒ๋ง ๊ธฐ์ตํ์ธ์.

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
    // ์ด๋ฐ ์์ผ๋ก
    this.setState((state) => ({
      count: state.count + amt,
    }));
  };
}
```

[TypeScript Playground์์ ํ์ธํด ๋ณด๊ธฐ](https://www.typescriptlang.org/play/?jsx=2#code/JYWwDg9gTgLgBAJQKYEMDG8BmUIjgcilQ3wFgAoCtAGxQGc64BBMMOJADxiQDsATRsnQwAdAGFckHrxgAeAN5wQSBigDmSAFxw6MKMB5q4AXwA0cRWggBXHjG09rIAEZIoJgHwWKcHTBTccAC8FnBWtvZwAAwmANw+cET8bgAUAJTe5L6+RDDWUDxwKQnZcLJ8wABucBA8YtTAaADWQfLpwV4wABbAdCIGaETKdikAjGnGHiWlFt29ImA4YH3KqhrGsz19ugFIIuF2xtO+sgD0FZVTWdlp8ddH1wNDMsFFKCCRji5uGUFe8tNTqc4A0mkg4HM6NNISI6EgYABlfzcFI7QJ-IoA66lA6RNF7XFwADUcHeMGmxjStwSxjuxiAA)

**Class Properties**: ๋ง์ฝ ๋์ค์ ์ฌ์ฉํ๊ธฐ ์ํด class properties๋ฅผ ์ ์ธํ๋ค๋ฉด, `state`์ ๊ฐ์ด ์ ์ธํ๋ ํ ๋น์ ํ์ง ์์ต๋๋ค.

```tsx
class App extends React.Component<{
  message: string;
}> {
  pointer: number; // ์ด๋ฐ ์์ผ๋ก
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

[TypeScript Playground์์ ํ์ธํด ๋ณด๊ธฐ](https://www.typescriptlang.org/play/?jsx=2#code/JYWwDg9gTgLgBAJQKYEMDG8BmUIjgcilQ3wFgAoCtAGxQGc64BBMMOJADxiQDsATRsnQwAdAGFckHrxgAeAN4U4cEEgYoA5kgBccOjCjAeGgNwUAvgD44i8sshHuUXTwCuIAEZIoJuAHo-OGpgAGskOBgAC2A6JTg0SQhpHhgAEWA+AFkIVxSACgBKGzjlKJiRBxTvOABeOABmMzs4cziifm9C4ublIhhXKB44PJLlOFk+YAA3S1GxmzK6CpwwJdV1LXM4FH4F6KXKp1aesdk-SZnRgqblY-MgA)

[์ถ๊ฐํ  ๋ด์ฉ์ด ์๋์? issue๋ฅผ ์์ฑํ์ธ์!](https://github.com/typescript-cheatsheets/react/issues/new).

#### getDerivedStateFromProps ํ์ํ(Typing) ํ๊ธฐ

`getDerivedStateFromProps`๋ฅผ ์ฌ์ฉํ๊ธฐ ์ ์, [documentation](https://reactjs.org/docs/react-component.html#static-getderivedstatefromprops)๊ณผ [You Probably Don't Need Derived State](https://reactjs.org/blog/2018/06/07/you-probably-dont-need-derived-state.html)๋ฅผ ์ฝ์ด๋ณด์ธ์. Derived State๋ memoization์ ์ค์ ํ๋ ๊ฒ์ ๋์ธ ์ ์๋ hooks์ ์ฌ์ฉํ์ฌ ๊ตฌํ๋  ์ ์์ต๋๋ค.

๋ค์์ `getDerivedStateFromProps`๋ฅผ annotateํ  ์ ์๋ ๋ช ๊ฐ์ง ๋ฐฉ๋ฒ์๋๋ค.

1. ๋ง์ฝ derived state์ type์ ๋ช์์ ์ผ๋ก ์ค์ ํ๊ณ , `getDerivedStateFromProps`์ return ๊ฐ์ด ์ค์ ํ type์ ์ค์ํ๋์ง ์๊ณ ์ถ์ ๊ฒฝ์ฐ

```tsx
class Comp extends React.Component<Props, State> {
  static getDerivedStateFromProps(props: Props, state: State): Partial<State> | null {
    //
  }
}
```

2. ํจ์์ return ๊ฐ์ด state๋ฅผ ๊ฒฐ์ ํ๋๋ก ํ๊ณ ์ถ์ ๊ฒฝ์ฐ

```tsx
class Comp extends React.Component<Props, ReturnType<typeof Comp["getDerivedStateFromProps"]>> {
  static getDerivedStateFromProps(props: Props) {}
}
```

3. ๋ค๋ฅธ state fields์ derived state ๊ทธ๋ฆฌ๊ณ  memoization์ ์ํ  ๊ฒฝ์ฐ

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

[TypeScript Playground์์ ํ์ธํด ๋ณด๊ธฐ](https://www.typescriptlang.org/play/?jsx=2#code/JYWwDg9gTgLgBAJQKYEMDG8BmUIjgcilQ3wFgAoUSWOYAZwFEBHAVxQBs5tcD2IATFHQAWAOnpJWHMuQowAnmCRwAwizoxcANQ4tlAXjgoAdvIDcFYMZhIomdMoAKOMHTgBvCnDhgXAQQAuVXVNEB12PQtyAF9La1t7NGUAESRMKyR+AGUYFBsPLzgIGGFbHLykADFgJHZ+II0oKwBzKNjyBSU4cvzDVPTjTJ7lADJEJBgWKGMAFUUkAB5OpAhMOBgoEzpMaBBnCFcZiGGAPijMFmMMYAhjdc3jbd39w+PcmwAKXwO6IJe6ACUBXI3iIk2mwO83joKAAbpkXoEfC46KJvmA-AAaOAAehxcBh8K40DgICQIAgwAAXnkbsZCt5+LZgPDsu8kEF0aj0X5CtE2hQ0OwhG4VLgwHAkAAPGzGfhuZDoGCiRxTJBi8C3JDWBb-bGnSFwNC3RosDDQL4ov4ooGeEFQugsJRQS0-AFRKHrYT0UQaCpwQx2z3eYqlKDDaq1epwABEAEYAEwAZhjmIZUNEmY2Wx2UD2KKOw1drgB6f5fMKfpgwDQcGaE1STVZEZw+Z+xd+cD1BPZQWGtvTwDWH3ozDY7A7aP82KrSF9cIR-gBQLBUzuxhY7HYHqhq4h2ceubbryLXPdFZiQA)

<!--END-SECTION:class-components-->

<!--START-SECTION:default-props-->

#### `defaultProps`๊ฐ ํ์ํ์ง ์์์๋ ์์ต๋๋ค

[์ด ํธ์](https://twitter.com/dan_abramov/status/1133878326358171650)์ ๋ฐ๋ฅด๋ฉด, defaultProps๋ deprecate ๋  ๊ฒ์๋๋ค.. ๋ค์์ ํ ๋ก ์ ํ์ธํด ๋ณด์ธ์.:

- [Original tweet](https://twitter.com/hswolff/status/1133759319571345408)
- [์ด article](https://medium.com/@matanbobi/react-defaultprops-is-dying-whos-the-contender-443c19d9e7f1)์์ ๋ ๋ง์ ์ ๋ณด๋ฅผ ์ป์ ์ ์์ต๋๋ค.

object default value๋ฅผ ์ฌ์ฉํ๋ ๊ฒ์ด ํต์์ ์ผ๋ก ํฉ์๋ ๋ด์ฉ์๋๋ค.

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

#### `defaultProps` ํ์ดํ ํ๊ธฐ

[TypeScript 3.0+](https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-0.html)์์ ํ์ ์ถ๋ก ์ ์ฑ๋ฅ์ด ๋งค์ฐ ๋ง์ด ๋ฐ์ ๋์์ต๋๋ค. ํ์ง๋ง ์ฌ์ ํ [๋ช๋ช์ edge case ๋ค์ด ๋ฌธ์ ๊ฐ ๋๊ธฐ๋ ํฉ๋๋ค.](https://github.com/typescript-cheatsheets/react/issues/61).

**Function Components**

```tsx
// ์ฌ์ด ๋ฐฉ๋ฒ์ผ๋ก typeof๋ฅผ ์ฌ์ฉํ  ์ ์์ต๋๋ค.; hoist๋๋ ๊ฒ์ ์ฃผ์ํ์ธ์!
// DefaultProps์ ์ ์ธํ  ์๋ ์์ต๋๋ค.
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

_[TS Playground์์ ํ์ธํด๋ณด๊ธฐ](https://www.typescriptlang.org/play?#code/JYWwDg9gTgLgBAKjgQwM5wEoFNkGN4BmUEIcARFDvmQNwBQdMAnmFnAOKVYwAKxY6ALxwA3igDmWAFxwAdgFcQAIyxQ4AXzgAyOM1YQCcACZYCyeQBte-VPVwRZqeCbOXrEAXGEi6cCdLgAJgBGABo6dXo6e0d4TixuLzgACjAbGXjuPg9UAEovAD5RXzhKGHkoWTgAHiNgADcCkTScgDpkSTgAeiQFZVVELvVqrrrGiPpMmFaXcytsz2FZtwXbOiA)_

**Class components**์ ๊ฒฝ์ฐ, ํ์ดํ์ ์ํ [๋ ๊ฐ์ง ๋ฐฉ๋ฒ](https://github.com/typescript-cheatsheets/react/pull/103#issuecomment-481061483) (including using the `Pick` utility type)์ด ์์ง๋ง, props definition์ ๊ฑฐ๊พธ๋ก ์ํ("reverse") ํ๋ ๊ฒ์ ์ถ์ฒํฉ๋๋ค.

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

// Type-checks! type assertion์ด ํ์ ์์!
let el = <Greet age={3} />;
```

<details>
<summary>๋ผ์ด๋ธ๋ฌ๋ฆฌ ์์ฑ์๋ฅผ ์ํ<b><code>JSX.LibraryManagedAttributes</code> ๋์์ค</b></summary>

์์์ ์๊ฐ๋ ๊ตฌํ์ ์ฑ ๊ฐ๋ฐ์๋ค์ด ์ฌ์ฉํ๋๋ฐ ์๋ฌด๋ฐ ๋ฌธ์ ๊ฐ ์์ต๋๋ค. ํ์ง๋ง ๋ค๋ฅธ ์ฌ๋๋ค์ด ์ฌ์ฉ(consume)ํ  ์ ์๋๋ก `GreetProps`๋ฅผ export ํ๊ณ ์ถ์ ๊ฒฝ์ฐ๋ ์์ต๋๋ค. ์ฌ๊ธฐ์ `GreetProps`๊ฐ ์ ์๋๋ ๋ฐฉ๋ฒ์ด ๋ฌธ์ ๊ฐ ๋ฉ๋๋ค. `age`๋ ๊ผญ ํ์ํ์ง ์์ ๋์๋ `defaultProps`๋๋ฌธ์ ํ์์ ์ธ props๊ฐ ๋ฉ๋๋ค.

[`GreetProps`๋ ๋น์ ์ ์ปดํฌ๋ํธ๋ฅผ ์ํ _๋ด๋ถ์ ์ธ_ ๊ท์น(์ปดํฌ๋ํธ๊ฐ ๊ตฌํํ๋ ๊ฒ)์ด์ง, _์ธ๋ถ์ ์ธ_ ๊ฒ์ด ์๋๋๋ค](https://github.com/typescript-cheatsheets/react/issues/66#issuecomment-453878710). ๋ฐ๋ผ์ export๋ฅผ ์ํ type์ ๋ฐ๋ก ๋ง๋ค ๊ฑฐ๋, `JSX.LibraryManagedAttributes` utility๋ฅผ ์ฌ์ฉํ  ์๋ ์์ต๋๋ค.

```tsx
// internal contract(๋ด๋ถ์ ์ธ ๊ท์น), export ๋์ด์๋ ์๋๋ค
type GreetProps = {
  age: number;
};

class Greet extends Component<GreetProps> {
  static defaultProps = { age: 21 };
}

// external contract(์ธ๋ถ์ ์ธ ๊ท์น)
export type ApparentGreetProps = JSX.LibraryManagedAttributes<typeof Greet, GreetProps>;
```

์ด๋ ๊ฒ ํ๋ฉด ์ฝ๋๊ฐ ์ ์คํ๋์ง๋ง, `ApparentGreetProps`๋ฅผ ์ฌ์ฉํ๋๊ฒ ๋ค์ ๋ฒ๊ฑฐ๋ก์ธ ์ ์์ต๋๋ค. ์๋์์ ์ค๋ชํ๋ `ComponentProps` utility๋ก boilerplate๋ฅผ ๊ฐ๋จํ๊ฒ ๋ง๋ค ์ ์์ต๋๋ค.

</details>

#### defaultProps๊ฐ ์๋ Component์ props๋ฅผ ์ฌ์ฉ(consume)ํ๊ธฐ

`defaultProps`๊ฐ ์๋ ์ปดํฌ๋ํธ๋ ์ค์ ๋ก๋ ๊ทธ๋ ์ง ์์ง๋ง ํ์์ ์ธ props๋ฅผ ๊ฐ์ง๋ ๊ฒ์ฒ๋ผ ๋ณด์ผ ์ ์์ต๋๋ค.

##### Problem Statement

๋ค์๊ณผ ๊ฐ์ ์์์ ํ๊ณ ์ถ๋ค๋ฉด,

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

// 'age' property๋ '{ name: string; }'์ ์์ง๋ง, '{ age: number; } type์์๋ ํ์์ ์ธ property ์๋๋ค.
const el = <TestComponent name="foo" />;
```

##### Solution

`JSX.LibraryManagedAttributes`๋ฅผ ์ ์ฉํ๋ ์ ํธ๋ฆฌํฐ๋ฅผ ์ ์ํฉ๋๋ค.

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

[_TS Playground์์ ํ์ธํด ๋ณด๊ธฐ_](https://www.typescriptlang.org/play?#code/JYWwDg9gTgLgBAKjgQwM5wEoFNkGN4BmUEIcARFDvmQNwBQdMAnmFnAMImQB2W3MABWJhUAHgAqAPjgBeOOLhYAHjD4ATdNjwwAdJ3ARe-cSyyjg3AlihwB0gD6Yqu-Tz4xzl67cl04cAH44ACkAZQANHQAZYAAjKGQoJgBZZG5kAHMsNQBBGBgoOIBXVTFxABofPzgALjheADdrejoLVSgCPDYASSEIETgAb2r0kCw61AKLDPoAXzpcQ0m4NSxOooAbQWF0OWH-TPG4ACYAVnK6WfpF7mWAcUosGFdDd1k4AApB+uQxysO4LM6r0dnAAGRwZisCAEFZrZCbbb9VAASlk0g+1VEamADUkgwABgAJLAbDYQSogJg-MZwYDoAAkg1GWFmlSZh1mBNmogA9Di8XQUfQHlgni8jLpVustn0BnJpQjZTsWrzeXANsh2gwbstxFhJhK3nIPmAdnUjfw5WIoVgYXBReKuK9+JI0TJpPs4JQYEUoNw4KIABYARjgvN8VwYargADkIIooMQoAslvBSe8JAbns7JTSsDIyAQIBAyOHJDQgA)

#### ์ฌ๋ฌ๊ฐ์ง ํ ๋ก ๊ณผ ์ง์

<details>
<summary><b><code>React.FC</code>๋ ์ <code>defaultProps</code>์ด ๋์ํ์ง ๋ชปํ๊ฒ ๋ง๋ค๊น์?</b></summary>

๋ค์์ ํ ๋ก ์ ํ์ธํด ๋ณด์ธ์.:

- https://medium.com/@martin_hotell/10-typescript-pro-tips-patterns-with-or-without-react-5799488d6680
- https://github.com/DefinitelyTyped/DefinitelyTyped/issues/30695
- https://github.com/typescript-cheatsheets/react/issues/87

์ด๊ฑด ํ์ฌ ์ํ์ผ ๋ฟ์ด๊ณ , ์ถํ์๋ ์ฌ๋ฐ๋ฅด๊ฒ ์์ ๋  ๊ฒ์๋๋ค.

</details>

<details>
<summary><b>TypeScript 2.9 and earlier</b></summary>

TypeScript 2.9์ ๊ทธ ์ด์  ๋ฒ์ ์์๋ ์ด๋ฌธ์ ๋ฅผ ํด๊ฒฐํ๋ ๋ฐฉ๋ฒ์ด ๋ค์ํฉ๋๋ค. ํ์ง๋ง ๋ค์ ๋ฐฉ๋ฒ์ด ์ฌํ๊น์ง ํ์ธํ ๋ฐฉ๋ฒ ์ค ๊ฐ์ฅ ์ข์ ๋ฐฉ๋ฒ์๋๋ค.

```ts
type Props = Required<typeof MyComponent.defaultProps> & {
  /* ์ถ๊ฐ์ ์ธ props */
};

export class MyComponent extends React.Component<Props> {
  static defaultProps = {
    foo: "foo",
  };
}
```

์ด์ ์๋ TypeScript์ `Partial type` ๊ธฐ๋ฅ์ ์ฌ์ฉํ๋ ๊ฒ์ด ๊ถ์ฅ ์ฌํญ์ด์๋๋ฐ, ์ด๋ ํ์ฌ ์ธํฐํ์ด์ค๊ฐ ๋ํ๋ ์ธํฐํ์ด์ค์์์ ๋ถ๋ถ์ ์ธ ๋ฒ์ ์ ์ถฉ์กฑํ๋ค๋ ๊ฒ์ ์๋ฏธํฉ๋๋ค. ์ด๋ฐ ๋ฐฉ๋ฒ์ผ๋ก type์ ๋ณ๊ฒฝํ์ง ์๊ณ  defaultProps๋ฅผ ํ์ฅํ  ์ ์์ต๋๋ค.

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

์ด ์ ๊ทผ ๋ฐฉ๋ฒ์ ๋ฌธ์ ์ ์ `JSX.LibraryManagedAttributes`๋ก ์๋ํ๋ ํ์ ์ถ๋ก ์ ๋ณต์กํ ์ด์๋ฅผ ๋ฐ์์ํจ๋ค๋ ๊ฒ์๋๋ค. ๊ธฐ๋ณธ์ ์ผ๋ก ์ปดํ์ผ๋ฌ๋ ํด๋น ์ปดํฌ๋ํธ๋ก JSX expression์ ์์ฑํ  ๋ ๋ชจ๋  props๊ฐ ์ ํ์ฌํญ(optional)์ด๋ผ๊ณ  ์๊ฐํฉ๋๋ค.

[@ferdaber์ ์๊ฒฌ์ ํ์ธํด ๋ณด์ธ์.](https://github.com/typescript-cheatsheets/react/issues/57) and [here](https://github.com/typescript-cheatsheets/react/issues/61).

</details>

[์ถ๊ฐํ  ๋ด์ฉ์ด ์๋์? ์ด์๋ฅผ ์์ฑํ์ธ์!](https://github.com/typescript-cheatsheets/react/issues/new).

<!--END-SECTION:default-props-->
