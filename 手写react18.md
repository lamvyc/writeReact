> 手写react18卡颂版

## 搭架子



```js
pnpm相比其他打包工具的优势:
·依赖安装快
·更规范（处理幽灵依赖问题）

参考资料:pnpm是凭什么对npm和yarn降维打击的？


安装
npm install -g pnpm
pnpm init

定义开发规范
pnpm i eslint -D -w
npx eslint --init
//报错了
pnpm i -D -w @typescript-eslint/eslint-plugin, @typescript-eslint/parser

pnpm i -D -w typescript @
typescript-eslint/eslint-plugin@5.6.0 @typescript-eslint/parser@5.6.0 eslint@7.32.0     

pnpm i -D -w typescript
pnpm i prettier -D -w 

//避免eslint与prettier冲突
pnpm i eslint-config-prettier eslint-plugin-prettier -D -w
//安装husky拦截commit命令
pnpm i husky -D -w
npx husky install
npx husky add .husky/pre-commit "pnpm lint"

//对commit信息进行规范
pnpm i commitlint @commit
lint/cli @commitlint/config-conventional -D -w

```

