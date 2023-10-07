<template>
    <div class="min-h-screen flex flex-col items-center justify-center bg-gray-100">
      <div class="bg-white p-8 rounded-lg shadow-md w-3/4 text-center">
        <h1 class="text-2xl mb-4">歡迎使用 vue-electron-vite-tailwind 模板</h1>
        <p class="mb-4">可查看以下連結來了解相關功能：</p>
        <a @click="openInNewWindow('https://vitejs.dev/')" class="underline hover:text-blue-600 cursor-pointer">Vite</a>
        <span> | </span>
        <a @click="openInNewWindow('https://vuejs.org/')" class="underline hover:text-blue-600 cursor-pointer">Vue3</a>
        <span> | </span>
        <a @click="openInNewWindow('https://electronjs.org/')" class="underline hover:text-blue-600 cursor-pointer">Electron</a>
        <span> | </span>
        <a @click="openInNewWindow('https://electron-vite.org/')" class="underline hover:text-blue-600 cursor-pointer">Electron-Vite</a>
        <span> | </span>
        <a @click="openInNewWindow('https://tailwindcss.com/')" class="underline hover:text-blue-600 cursor-pointer">Tailwind CSS</a>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'App',
    methods: {
      openInNewWindow(url) {
        window.electron.openExternal(url);
      }
    }
  }
  </script>
  
  <style scoped>
  /* 可以在此處添加更多的 TailwindCSS 樣式或自定義樣式 */
  </style>
  