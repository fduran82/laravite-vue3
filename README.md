<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

## About Laravite-vue3

Just a simple way to start a laravel vite project with vuejs.

- create new laravel app
```
$ laravel new laravite-vue3
```
- cd into the project.
- add in tag head vite 
```
 @vite(['resources/css/app.css', 'resources/js/app.js'])
```
- go to view welcome blade and delete all inside body tag. create a div with id app.
```
    <body class="antialiased">
        <div id="app"></div>
    </body>
```
- now lets install vue and plugin vitejs
```
$ npm i vue@next -D
$ npm i @vitejs/plugin-vue -D
```
- import vue on vite.config file
```
    import { defineConfig } from 'vite';
    import laravel from 'laravel-vite-plugin';
    import vue from '@vitejs/plugin-vue';

    export default defineConfig({
        plugins: [
            laravel({
                input: ['resources/css/app.css', 'resources/js/app.js'],
                refresh: true,
            }),
            vue({
                template: {
                    transformAssetUrls: {
                        base: null,
                        includeAbsolute: false,
                    }
                }
            }),
        ],
    });

```
- go to resources js folder and create a Welcome.vue file. Just put a welcome text like:
```
<template>
  <h1>Welcome from vuejs</h1>
</template>
```
- go to resources js folder and open app.js delete all and add: 
```
import { createApp } from 'vue';
import Welcome from './Welcome.vue';


createApp(Welcome).mount('#app');

```
- open a terminal on project and run:
```
$ npm run dev
```
- All set!, now open the app on web browser and you should see thw welcome text from vue.




Happy Coding!  :computer:  See you all! Bye  👋
**[Fidel Duran](https://fidelduran.com)** 

<p align="center"><a href="https://fidelduran.com" target="_blank"><img width="150" src="https://fidelduran.com/images/logos/logo-yellow.svg"></a></p>

