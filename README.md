
# vue-electron-vite-tailwind

## 簡介

`vue-electron-vite-tailwind` 是一個結合 Electron, Vue 3 和 TailwindCSS 的開箱即用模板。這個模板可以快速地幫助開發者建立 Electron 桌面應用。

這是使用 JavaScript 的模板（太多TypeScript的模板，我不會啊！），如果你想使用 TypeScript，可以找其他的模板。

## 功能

- 使用 [`Vite`](https://vitejs.dev/) 作為建構工具
- 整合 [`Vue 3`](https://vuejs.org/) 作為前端框架
- 使用 [`TailwindCSS`](https://tailwindcss.com/) 進行風格設計
- 透過 [`electron-vite`](https://electron-vite.org/) 進行 Electron 應用的開發和打包

## 目錄結構

```
.
├── build                     # 包含應用圖標和其他打包資源
├── electron-builder.yml      # Electron builder 的配置文件
├── electron.vite.config.js   # Vite 的配置文件
├── package-lock.json         # NPM 鎖定版本文件
├── package.json              # 專案描述和依賴文件
├── postcss.config.js         # PostCSS 的配置文件
├── README.md                 # README 文件
├── resources                 # 其他資源文件
└── src                       # 原始碼目錄
    ├── main                  # Electron 主程序
    ├── preload               # Electron 預加載腳本
    └── renderer              # Electron 渲染程序 (使用 Vue)
        ├── assets            # 靜態資源
        ├── src               # Vue 原始碼
        └── index.html        # HTML 入口
```

## 開始使用

1. 克隆此專案：  
   `git clone [此專案網址]`

2. 安裝依賴：  
   `npm install`

3. 啟動開發伺服器：  
   `npm run dev`

4. 打包應用：  
   - Windows: `npm run build:win`
   - macOS: `npm run build:mac`
   - Linux: `npm run build:linux`

   打包後的應用會被保存在 `/dist` 目錄中。

## 依賴和版本

- 主要依賴：
  - `electron`: ^25.6.0

- 開發依賴：
  - `electron-vite`: ^1.0.27
  - `vite`: ^4.4.9
  - `vue`: ^3.3.4
  - `tailwindcss`: ^3.3.3

## 配置

- `electron.vite.config.js`: Vite 的配置文件，包含主程序、預加載和渲染程序的設定。
- `postcss.config.js`: PostCSS 的配置文件。
- `tailwind.config.js`: TailwindCSS 的配置文件。

## 貢獻

歡迎向此專案貢獻！