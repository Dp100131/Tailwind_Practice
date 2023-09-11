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

### Grid 
Cuadrícula compuesta de filas y columnas.