## 0.7.0 (2024-04-21)

- 0dcdf39 chore: remove `globalThis.__dirname`
- f48de08 feat: add `.npmrc` to template
- 9c84030 feat: support esmodule
- e2c3822 chore: bump deps

## 0.6.0 (2024-04-18)

- 28f7b4a fix: compatible vitest #26
- b0f59fb (github/v0.6.0) chore: update electron-builder.json5
- 59d3d33 refactor: better `process.env` assign
- e636b5d chore: correct `process.env.VITE_PUBLIC`

## 0.5.2 (2024-03-29)

- 73fecf2 Merge pull request #33 from badspider7/patch-1
- 2797dc2 fix: resolve ipcRenderer no returns
- fcfc74d (tag: v0.5.0) v0.5.1
- 77d76f4 fix: includes template-*/** to files

## 0.5.0 (2024-03-17)

- 626ed65 v0.5.0
- 742b923 chore: sync templates form create-vite
- c8d33a9 chore: bupms electron, electron-builder, vite-plugin-electron
- 232c526 feat: preload.ts adapt electron@29
- a9e13ae feat: add create-electron-vite.gif

## 0.4.0 (2023-09-06)

- 38af79d chore: test v0.4.0
- f5dafdf chore: update template
- 7114cac chore: site use `https://electron-vite.github.io`
- 394686c refactor: use `vite-plugin-electron` simple API

#### Main Changed

**0.4.0** use the simple API of `vite-plugin-electron`

```ts
import electron from 'vite-plugin-electron/simple'

electron({
  main: {
    entry: 'electron/main.ts',
  },
  preload: {
    input: __dirname + '/electron/preload.ts',
  },
  renderer: {},
})
```

**0.3.0**

```ts
import electron from 'vite-plugin-electron'

electron([
  {
    entry: 'electron/main.ts',
  },
  {
    entry: 'electron/preload.ts',
  },
])
```

## 0.3.0 (2023-05-27)

42dc950 refactor: use Vite instead unbuild
246cdfd feat(0.3.0): electron files
b1a194c feat(0.3.0): fully based on `create-vite` template
b6e5cb3 feat: template-react-ts, template-vanilla-ts, template-vue-ts

## 0.2.3 (2023-03-13)

#### Main Changed

- 05f9a47 fix: remove `.git` after clone

## 0.2.2 -> 0.2.3

## 0.2.1 (2023-03-13)

#### Main Changed

- 8d52193 feat: support create project into exists directory | [see here](https://github.com/vitejs/vite/pull/12390#issuecomment-1465457917)
