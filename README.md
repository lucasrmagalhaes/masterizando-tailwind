Tailwind

Projeto
pnpm create next-app tailwind-next

Height
h-full - 100%
h-screen - 100vh

Width
max-w-2xl

Font
font-bold

Before
flex items-center gap-3 before:w-0.5 before:h-8 before:bg-sky-500 before:flex - carregar o elemento antes do elemento

Button
rounded
enabled:hover:bg-sky-400
disabled:opacity-60
disabled:cursor-not-allowed

Responsividade
mobile first
sm 640px pra cima
md 768 pra cima
lg 1024px pra cima
xl 1280px pra cima
2xl 1536 pra cima

Tema - Light e Dark
dark:text-state-400

Valores Arbitrários
max-w-[400px]
bg-[#FFF]

tailwind.config.js
```
theme: {
	extend: {
		maxWidth: {
			exemplo: ‘700px'
		}
	}
}

// max-w-app
```

Configurando ESLint e Prettier
pnpm i prettier plugin tailwindcss -D

package.json
```
  "devDependencies": {
    "@rocketseat/eslint-config": "^2.1.0",
    "prettier-plugin-tailwindcss": "^0.4.1"
  }
```

prettier.config.js
```
module.exports = {
  plugins: [require('prettier-plugin-tailwindcss')],
}
```

Quando salva faz os ajustes
```
“editor.codeActionsOnSave”: {
	“source.fixAll.eslint”: true
}
```

layout.tsx
```
<body>
	<div className=“min-h-screen”>
		<main>
			{children}
		</main>
	</div>
</body>
```

Grid
```
gridTemplateColumns: {
	app: ‘minmax(18rem, 20rem) 1fr'
}

// grid grid-cols-app
```

Border
border-r border-zinc-200

[ignite-masterclass-tailwind-next](https://github.com/rocketseat-education/ignite-masterclass-tailwind-next)
