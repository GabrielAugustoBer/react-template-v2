# 🚀 React Template v2 - Guia Rápido

## Sobre o Projeto
Esse template é perfeito para quem quer iniciar um projeto React moderno de forma rápida e eficiente. Ele já vem com Vite, TypeScript e Tailwind CSS prontos para uso. Além disso, o Biome ajuda a manter o código limpo e organizado.

## O que tem nesse template?
- **React 19** - A biblioteca mais usada para construir interfaces.
- **Vite 6** - Build ultrarrápida para devs modernos.
- **TypeScript 5.7** - Tipagem forte para evitar bugs.
- **Tailwind CSS 4** - Estilização rápida e flexível.
- **Biome** - Ferramenta para deixar seu código bonito e bem formatado.

## Como rodar o projeto?
Aqui estão alguns comandos úteis:

```sh
npm run dev      # Inicia o servidor de desenvolvimento
npm run build    # Gera os arquivos para produção
npm run preview  # Visualiza a versão final do app
```

## Como começar?
1. Clone o repositório:
   ```sh
   git clone https://github.com/seu-usuario/react-template-v2.git
   ```
2. Entre no diretório do projeto:
   ```sh
   cd react-template-v2
   ```
3. Instale as dependências:
   ```sh
   npm install
   ```
4. Rode o servidor de desenvolvimento:
   ```sh
   npm run dev
   ```

## Tailwind CSS já está pronto!
O Tailwind já está configurado, então basta importar o arquivo CSS no `main.tsx` e começar a usar as classes:

```tsx
import "./index.css";
```

## Configuração do Vite
Já vem tudo pronto para React e Tailwind no `vite.config.ts`:

```ts
import path from "path"
import react from "@vitejs/plugin-react"
import { defineConfig } from "vite"
import tailwindcss from "@tailwindcss/vite"

export default defineConfig({
  plugins: [react(), tailwindcss()],
  resolve: {
    alias: {
      "@": path.resolve(__dirname, "./src"),
    },
  },
})
```

## Novas Configurações do TypeScript
Agora você pode usar `@` para importar qualquer arquivo dentro de `src` sem precisar de caminhos relativos longos. Por exemplo:

```tsx
import Button from "@/components/Button";
```

Isso facilita a organização do código e torna as importações mais limpas e eficientes!

## Quer contribuir?
Fique à vontade para fazer um fork do projeto, criar sua branch e mandar um pull request! 

## Licença
Este projeto está sob a [MIT License](LICENSE).
