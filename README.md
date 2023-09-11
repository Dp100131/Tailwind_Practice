# Comandos:
```
npm install -D tailwindcss
npx tailwindcss init
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```
# Tailwind

## Directivas de Tailwind

- ### @Tailwind base.
- ### @tailwind components.
- ### @tailwind utilities.
- ### @apply.
- ### @layer.
- ### @variants.
- ### @Responsive.
- ### @screen.
- ### theme().


## Colores

[Colors.]url('https://tailwindcss.com/docs/customizing-colors')

## Medidas y Breakpoints

### Breakpoint:
- sm md xl.
### Medidas
- w-5 -> En rem.
- w-1/2 -> %.
- w-full - viewport.

```
<div class="w-auto h-96 bg-sky-200 flex">
    <div class="w-1/4 h-1/2 bg-sky-700"></div>
    <div class="w-1/4 h-1/4 bg-cyan-400"></div>
    <div class="w-1/4 h-3/4 bg-cyan-700"></div>
    <div class="w-1/4 h-100 bg-cyan-900"></div>
</div>
```

## Flexbox y grid

### Flex
row o column.

```
<div class="w-96 h-96 bg-gray-100 p-10 m-20 flex flex-col gap-y-4 justify-center items-center">
    <div class="w-16 h-16 bg-red-300"></div>
    <div class="w-16 h-16 bg-red-300"></div>
    <div class="w-16 h-16 bg-red-300"></div>
    <div class="w-16 h-16 bg-red-300"></div>
</div>
```

### Grid 
Cuadrícula compuesta de filas y columnas.

## Personalización

```
tailwind.config.js

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}", "./public/**/*.{html,js}"],
  theme: {
    fontFamily: {
      'Montserrat': ["Montserrat", "sans-serif"]
    },
    backgroundColor: theme => ({
      ...theme('colors'),
      'primary': '#CC2D4A',
      'secondary': '#8FA206',
      'tertiary': '#61AEC9',
    }),
    textColor: theme => ({
      ...theme('colors'),
      'primary': '#CC2D4A',
      'secondary': '#8FA206',
      'tertiary': '#61AEC9',
    }),
    extend: {
      backgroundImage: {
        'sanFrancisco': "url('./public/img/sanFrancisco.jpg')",
        'sanFranciscoDesktop': "url('./public/img/sanFranciscoDesktop.jpg')",
        'bali': "url('./public/img/bali.jpg')",
        'chicago': "url('./public/img/chicago.jpg')",
        'europe': "url('./public/img/europe.jpg')",
        'iceland': "url('./public/img/iceland.jpg')",
        'LA': "url('./public/img/LA.jpg')",
        'miami': "url('./public/img/miami.jpg')",
        'new_york': "url('./public/img/new_york.jpg')",
        'norway': "url('./public/img/norway.jpg')",
        'seattle': "url('./public/img/seattle.jpg')",
        'switzerland': "url('./public/img/switzerland.jpg')",
        'sydney': "url('./public/img/sydney.jpg')",
        'yosemite': "url('./public/img/yosemite.jpg')",
      },
    },
  },
  plugins: [],
}
```