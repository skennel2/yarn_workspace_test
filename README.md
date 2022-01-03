### error Workspaces can only be enabled in private projects.  
yarn workspace는 private 프로젝트에서만 동작하는듯하다. (이 제약은 2.0.0릴리즈에서 제거되었다고 함.)
워크스페이스 프로젝트 루트 package.json에 "private": "true"넣어서 해결 

```
private: true의 정확한 의미는?  
npm Repository에 배포되지 않는 프로젝트 (공식 배포용이 아님)
```

### (node:73243) Warning: To load an ES module, set "type": "module" in the package.json or use the .mjs extension.
node.js의 기본적인 모듈시스템은 CommonJs  
아래 링크에서 node.js에서 ES6모듈을 사용할 수 있는 방법을 알 수 있다.
https://www.daleseo.com/js-node-es-modules/
  
```
workspace 루트 package.json이 아닌 개별 프로젝트에서 변경  
workspace 루트에서만 변경했을때는 동작 안하는것 확인
```