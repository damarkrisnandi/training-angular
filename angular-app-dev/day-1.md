# Training Angular - Day 1

## Persiapan
Basic yang setidaknya harus dimiliki oleh Angular Developer
* HTML
* CSS
* Javascript
* Typescript

Tools yang diperlukan untuk mengembangkan dan menjalankan aplikasi framework Angular 
* NodeJS - [https://nodejs.org/](https://nodejs.org/)
* Angular CLI - [https://cli.angular.io/](https://cli.angular.io/)
* Visual Studio Code - [https://code.visualstudio.com/](https://code.visualstudio.com/)


Cek versi Node
```bash
node -v
```
Cek versi npm
```bash
npm -version
```

Cek versi Angular
```bash
ng v
```

## Hello World!
Membuat aplikasi baru
```bash
ng new hello-world
```

Menjalankan aplikasi hello-world
```bash
ng serve
```
**Note:** Pastikan menjalankan ng serve di dalam direktori yg telah di create di awal

## Architecture
* <b>Modules
* Components
* Services</b>

![picture alt](https://angular.io/generated/images/guide/architecture/overview2.png "Angular Achitecture")

Selengkapnya
[https://angular.io/guide/architecture](https://angular.io/guide/architecture)

### 1. Modules
Aplikasi yang dikembangkan dengan Angular bersifat modular dan memiliki <i>modularity system</i> yg bernama <b>@NgModule</b>. 

### 2. Components
Component adalah bagian yang membangun bagian fisik aplikasi. Component dalam Aplikasi Angular dapat dipecah-pecah dan dirangkai menjadi satu bagian utuh.

### 3. Service
Service adalah bagian yg bertanggung jawab dalam business logic

## Modules - Component - Service
Sebuah Module "membungkus" beberapa Component dan beberapa Service, dan memungkinkan untuk mendistribusikan component dan service tersebut ke component atau service lain baik di dalam module tersebut ataupun module lain

## Lebih dalam membahas Component
Component terbentuk dari:
* Template
* Class
* Metadata

### Membuat Component Baru
``` bash
ng g c NamaComponent
```
### Interpolation
Interpolation adalah proses penyisipan data ke dalam template. Interpolation ditandai dengan penggunaan double curly bracket ``{{...}}``.
``` typescript
template: `
 <h2>Hello {{ name }}</h2>
 <h2> {{ 1 + 1 }} </h2>
 <h2> {{ "Welcome " + name }} </h2>
 <h2> {{ name.length }} </h2>
 <h2> {{ name.toUpperCase() }} </h2>
 <h2> {{ halo() }} </h2>
 `,
styles: []

```