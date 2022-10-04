# poc-monorepo-react

Invalid Hook Issue가 이전에 발생했으나 현재 재현 안됨.

## SSR

node version 16.14.0 이하인 경우에는 빌드 시에 계속해서 pending 상태라면 `next.config.js` 에 아래 설정이 필요함.

```js
experimental: {
  workerThreads: true;
}
```

이상인 경우에는 필요 없음

## CSR
