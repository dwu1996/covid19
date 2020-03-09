# 東京都 COVID-19 應對措施官方網站
![](https://github.com/tokyo-metropolitan-gov/covid19/workflows/production%20deploy/badge.svg)

[![Tokyo COVID-19 Task Force website](https://user-images.githubusercontent.com/1301149/75629392-1d19d900-5c25-11ea-843d-2d4376e3a560.png)](https://stopcovid19.metro.tokyo.lg.jp/)

### [日本語](./README.md) | [English](./README_EN.md) | 繁體中文

## 我該如何做出貢獻？

我們歡迎來自各地的協助！
請點選 [如何做出貢獻](./.github/CONTRIBUTING_ZH.md) 來查看更多資訊。

## 行動目標與開發原則

請點選 [開發者規則](./.github/CODE_OF_CONDUCT_ZH.md) 來查看更多資訊。

## 授權條款
本軟體之授權條款由 [MIT License](./LICENSE.txt) 所規範。

## 給開發者的注意事項

### 如何設定開發環境？

- 需要 Node.js 版本: 10.19.0 或更新的版本

**使用 yarn 的情況**
``` bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev
```

**使用 docker 的情況**
```bash
# serve with hot reload at localhost:3000
$ docker-compose up --build
```

### 部署開發環境、測試環境與發佈網站更新

當 `master` 分支被更新，HTML 檔案會自動的建置到 `production` 分支，
並且官方網站 (https://stopcovid19.metro.tokyo.lg.jp/) 也會做出對應的更新。

當 `staging` 分支被更新，HTML 檔案會自動的建置到 `gh-pages` 分支，
並且測試中網站 (https://stg-covid19-tokyo.netlify.com/) 也會做出對應的更新。

當 `development` 分支被更新，HTML 檔案會自動的建置到 `dev-pages` 分支，
並且開發中網站 (https://dev-covid19-tokyo.netlify.com/) 也會做出對應的更新。
