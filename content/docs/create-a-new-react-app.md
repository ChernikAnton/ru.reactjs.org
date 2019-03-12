---
id: create-a-new-react-app
title: Create a New React App
permalink: docs/create-a-new-react-app.html
redirect_from:
  - "docs/add-react-to-a-new-app.html"
prev: add-react-to-a-website.html
next: cdn-links.html
---

Используйте встроенный набор инструментов для лучшего взаимодействия пользователя и разработчика. 

На этой странице описано несколько популярных наборов инструментов React, которые помогают в таких задачах как:

* Пересчёт большого количества файлов и компонентов.
* Использование сторонних библиотек из npm.
* Раннее обнаружение распространённых ошибок.
* Отслеживание изменений CSS и JS на лету в процессе разработки.
* Оптимизация кода для продакшена.

Рекомендованные на этой странице инструменты **не требуют дополнительной настройки для начала работы.**

## Вам не нужен дополнительный набор инструментов {#you-might-not-need-a-toolchain}

Если вы не испытываете проблем описанных выше или пока не чувствуете себя уверенно, используя инструменты JavaScript, рассмотрите возможность [добавления React в виде  простого тега `<script>` на HTML странице](/docs/add-react-to-a-website.html) , [при необходимости с JSX](/docs/add-react-to-a-website.html#optional-try-react-with-jsx).

Также это **самый простой способ добавить React в существующий веб-сайт**. Вы всегда можете расширить набор инструментов, если посчитаете это нужным.


## Рекомендуемый набор инструментов {#recommended-toolchains}

Команда React в первую очередь рекомендует следующие решения:

- Если вы **изучаете React** или **создаёте новое [одностраничное](/docs/glossary.html#single-page-application) приложение**, используйте [Create React App](#create-react-app).
- Если вы создаете **серверный сайт с Node.js,** попробуйте [Next.js](#nextjs).
- Если вы создаете **статический контент-ориентированный сайт,** попробуйте [Gatsby](#gatsby).
- Если вы создаете **библиотеку компонентов** или **интегрируетесь с существующей кодовой базой**, попробуйте [более гибкие наборы инструментов](#more-flexible-toolchains).

### Create React App {#create-react-app}

[Create React App](https://github.com/facebookincubator/create-react-app) – удобная среда для **изучения React** и лучший способ начать создание **нового [одностраничного](/docs/glossary.html#single-page-application) приложения** на React.

Инструмент настраивает среду разработки таким образом, чтобы вы можете использовать новейшие возможности JavaScript, предоставляет хороший опыт разработки и оптимизирует приложение для продакшена. Вам понадобится Node версии >= 6 и npm версии >= 5.2 на вашем компьютере. Для создания проекта выполните:

```bash
npx create-react-app my-app
cd my-app
npm start
```

>Примечание
>
>`npx` в первой строке не является опечаткой. Это [инструмент запуска пакетов, появившийся в npm версии 5.2+](https://medium.com/@maybekatz/introducing-npx-an-npm-package-runner-55f7d4bd282b).


Create React App не обрабатывает бэкенд логику или базы данных, он только предоставляет команды для сборки фронтенда, поэтому вы можете использовать его с любым бэкэндом. Внутри используются [Babel](https://babeljs.io/) и [webpack](https://webpack.js.org/), но вам не нужно ничего знать о них.

Когда ваше приложение готово к развёртыванию на продакшене, запуск команды `npm run build` создаст оптимизированную сборку вашего приложения в папке `build`. Вы можете узнать больше о Creat React App [из его README](https://github.com/facebookincubator/create-react-app#create-react-app-) и [его пользовательского руководства](https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md#table-of-contents).

### Next.js {#nextjs}


[Next.js](https://nextjs.org/) – это популярный и простой фреймворк для **статических и серверных приложений**, созданный с помощью React. Он включает в себя **готовые решения для стилизации и маршрутизации** и предполагает, что вы используете [Node.js](https://nodejs.org/) в качестве серверной среды.

Узнайте больше о Next.js из [его официального руководства](https://nextjs.org/learn/). 

### Gatsby {#gatsby}

[Gatsby](https://www.gatsbyjs.org/) – лучший способ для создания **статических сайтов** с помощью React. Он позволяет использовать React-компоненты, но выводит предварительно отрендеренный HTML и CSS, чтобы гарантировать самое быстрое время загрузки.

Узнайте больше о Gatsby из [его официального руководства](https://www.gatsbyjs.org/docs/) и [галереи стартовых комплектов](https://www.gatsbyjs.org/docs/gatsby-starters/).

### Более гибкие наборы инструментов {#more-flexible-toolchains}                             
Следующие наборы инструментов предлагают больше гибкости и выбора. Мы рекомендуем их более опытным разработчикам:


-**[Neutrino](https://neutrinojs.org/)** сочетает в себе мощь [webpack](https://webpack.js.org/) с простотой пресетов и включает в себя пресеты для [React-приложений](https://neutrinojs.org/packages/react/) и [ React-компонентов](https://neutrinojs.org/packages/react-components/) .

-**[nwb](https://github.com/insin/nwb)** особенно хорош для [публикации React-компонентов в npm](https://github.com/insin/nwb/blob/master/docs/guides/ReactComponents.md#developing-react-components-and-libraries-with-nwb). Его [также можно использовать](https://github.com/insin/nwb/blob/master/docs/guides/ReactApps.md#developing-react-apps-with-nwb) для создания React-приложений.

-**[Parcel](https://parceljs.org/)** – быстрый упаковщик веб-приложений с нулевой конфигурацией, [который работает с React](https://parceljs.org/recipes.html#react).


-**[Razzle](https://github.com/jaredpalmer/razzle)** – это фреймворк для серверного рендеринга, который не требует какой-либо настройки, но более гибкий, чем Next.js.


## Создание набора инструментов с нуля {#creating-a-toolchain-from-scratch}

Набор инструментов для сборки JavaScript обычно состоит из:


* **Менеджер пакетов**, такой как [Yarn](https://yarnpkg.com/) или [npm](https://www.npmjs.com/). Он позволяет вам использовать обширную экосистему сторонних пакетов и легко устанавливать или обновлять их.


* **Сборщик**, такой как [webpack](https://webpack.js.org/) или [Parcel](https://parceljs.org/). Он позволяет писать модульный код и объединять его в небольшие пакеты, чтобы оптимизировать время загрузки.


* **Компилятор**, такой как [Babel](https://babeljs.io/). Он позволяет писать современный код JavaScript, который также будет работать в старых браузерах.

Если вы предпочтёте создать свой собственный набор JavaScript-инструментов с нуля, [ознакомьтесь с этим руководством](https://blog.usejournal.com/creating-a-react-app-from-scratch-f3c693b84658), в котором воссоздаются некоторые функции Create React App.

Не забудьте убедиться, что ваш собственный набор инструментов [правильно настроен для продакшена](/docs/optimizing-performance.html#use-the-production-build).
