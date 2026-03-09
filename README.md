# Album de Fotos (React + Vite)

Aplicacao React que consome a API do Unsplash para:
- listar fotos aleatorias na tela inicial
- pesquisar fotos por texto
- filtrar por categorias
- abrir foto ampliada em modal

## Tecnologias
- React 18
- Vite 5
- Axios
- ESLint

## Requisitos
- Node.js 18+ (recomendado)
- npm
- chave de API do Unsplash

## Configuracao
1. Instale as dependencias:

```bash
npm install
```

2. Crie o arquivo `.env` na raiz do projeto:

```env
VITE_UNSPLASH_API_KEY=sua_chave_aqui
```

3. Rode o projeto em modo desenvolvimento:

```bash
npm run dev
```

## Scripts disponiveis
- `npm run dev`: inicia o servidor de desenvolvimento
- `npm run build`: gera build de producao
- `npm run preview`: executa preview do build
- `npm run lint`: roda validacao de codigo com ESLint

## Estrutura do projeto
```text
src/
  components/
    SearchBar.jsx
    FotoList.jsx
    Foto.jsx
    FotoAmpliada.jsx
  App.jsx
  main.jsx
```

## Como funciona
- Ao abrir a aplicacao, sao buscadas 10 fotos aleatorias no Unsplash.
- Quando voce pesquisa e/ou seleciona categoria, a busca usa `/search/photos`.
- Ao clicar em uma foto, ela abre ampliada em um modal.

## Seguranca
- Nao versione o arquivo `.env`.
- Mantenha `node_modules/` no `.gitignore`.

## Autor
Matheus Sousa
