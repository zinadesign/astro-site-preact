# Сайт на Astro с Tailwind, Preact, AOS и удобствами

На основе минималистичного шаблона Astro + Tailwind https://github.com/zinadesign/astro-tailwind

## Install

Использовать при установке Astro с параметром:

With NPM:

```bash
npm create astro@latest . -- --template zinadesign/astro-site-preact
```

With Yarn:

```bash
yarn create astro . --template zinadesign/astro-site-preact
```

Или в менее болтливом режиме:

```bash
npm create astro@latest . -- --template zinadesign/astro-site-preact --skip-houston --install --no-git
```

```bash
yarn create astro . --template zinadesign/astro-site-preact --skip-houston --install --no-git
```

Вместо точки можно писать имя папки проекта. Т.е. с точкой запускать внутри существующей папки проекта, а если с названием, то папка будет создана.

После установки запускать как обычно в Astro:

```bash
npm run dev
```

## Дополнительные возможности

* [Nesting](https://tailwindcss.com/docs/using-with-preprocessors#nesting) на основе встроенного в Tailwind плагина `postcss-nested`, для этого добавлен файл `postcss.config.cjs`
* [Prettier](https://prettier.io/) для форматирования классов Tailwind в файлах `.astro`, для этого добавлен файл `.prettierrc.json`
* [Preact](https://preactjs.com/) в качестве минимального (3 кб) JavaScript фреймворка, совместимого с React
* [AOS](https://michalsnik.github.io/aos/) для анимаций при прокрутке — см. `src/scripts/aos.js` и атрибуты типа `data-aos="fade-up"` у тегов HTML
* [Path Aliases](https://docs.astro.build/en/guides/aliases/) — см. `tsconfig.json`
