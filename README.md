# DRMConnect

Uma plataforma de perguntas e respostas feita por e para alunos. O conhecimento da DRM se conecta aqui.

Aplicação web em React + Vite, com autenticação e dados no Supabase.

## Requisitos

- [Node.js](https://nodejs.org) 20.19+ ou 22.12+ (versões exigidas pelo Vite 8) e npm

## Como instalar e rodar

### 1. Instale as dependências

```bash
npm install
```

### 2. Configure as variáveis de ambiente

Crie um arquivo `.env` na raiz do projeto com a URL e a chave pública (anon key) do projeto no Supabase:

```env
VITE_SUPABASE_URL=https://seu-projeto.supabase.co
VITE_SUPABASE_ANON_KEY=sua-chave-anon-publica
```

Os dois valores ficam no painel do Supabase, em **Settings → API** (*Project URL* e *Project API keys → anon public*). Sem esse arquivo a aplicação sobe, mas login e dados não funcionam. O `.env` não deve ser commitado — ele já está no `.gitignore`.

### 3. Rode em modo de desenvolvimento

```bash
npm run dev
```

A aplicação fica disponível em [http://localhost:5173](http://localhost:5173), com recarregamento automático a cada alteração.

### 4. Gere a versão de produção

```bash
npm run build
```

Os arquivos finais são gerados na pasta `dist/`.

### 5. Veja a versão de produção localmente

```bash
npm run preview
```

Serve a pasta `dist/` em [http://localhost:4173](http://localhost:4173), do mesmo jeito que ela vai para o ar.

## Outros comandos

```bash
npm run lint   # verifica o código com ESLint
```
