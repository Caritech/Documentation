# Convert Nuxt Js into Mobile App

## Reference

https://capacitorjs.com/blog/integrating-capacitorjs-plugins-with-nuxtjs

https://serversideup.net/packaging-a-nuxtjs-app-for-ios-and-android-with-capacitorjs/

## Software:

- CapacitorJS  (https://capacitorjs.com/solution/vue)
- Nuxt (https://nuxtjs.org/docs/2.x/get-started/installation)
- Android Studio (please keep the version latest)
- Node Js





## Walkthrough

- create a `nuxt` app

  ```
  npx create-nuxt-app my-app-1
  ```

  ```
  Project name: (Press Entter to use back project name)
  Programming Language: JavaScript
  Package Manager: Npm
  UI framework: TailwindCss (recommended)
  Nuxt.js modules: Axios + PWA
  Linting tools:  ESLint / Prettier
  Testing framework: none
  Rendering mode: Single Page App
  Deployment target: Static
  Deployment Tools: jsconfig.json
  Continuous integration: None
  Version controler system: Git
  ```

- run command to create `dist` directory

  ```
  cd my-app-1
  npm run generate
  ```

  ###  Install Capacitor Plugin

- ```
  npm install @capacitor/core @capacitor/cli
  npx cap init my-app-1 com.example.app --web-dir=dist
  
  npm i @capacitor/ios @capacitor/android
  
  npx cap add android
  npx cap add ios 
  ```

- ```
  npx cap copy
  
  npx cap open android
  ```

  - Android studio will open
  - Wait for gradle to download
  - click "Play" button to start emulator



