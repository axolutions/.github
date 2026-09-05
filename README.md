# Site institucional da Axolutions
Repositório do site institucional da Axolutions, com foco em conteúdo institucional e catálogo de serviços.

## Sobre
A Axolutions é uma startup brasileira de desenvolvimento de software sediada em São Paulo (CNPJ 60.140.588/0001-00).

Este projeto reúne o site institucional da empresa. A Axolutions desenvolve sites, sistemas web, aplicativos, e-commerces e automações sob medida. O diferencial operacional é entregar uma prévia funcional no mesmo dia, sem custo e sem compromisso.

## Stack
- **Framework:** Next.js 14 (App Router)
- **Linguagem:** TypeScript
- **Estilo:** Tailwind CSS
- **Deploy:** estático
- **Node.js (mínimo):** `>=18.17.0`
- **Gerenciador de pacotes (mínimo):** `npm >=9.0.0` (`TODO`: confirmar versão oficial quando `package.json`/lockfile existir)

## Rodando localmente
1) Clonar o repositório:

```bash
git clone https://github.com/axolutions/.github.git
cd .github
```

2) Instalar dependências:

```bash
npm install
```

3) Configurar variáveis de ambiente:

```bash
cp .env.example .env.local
```

> `TODO`: criar/validar `.env.example` e documentar as variáveis obrigatórias de produção e desenvolvimento.

4) Subir ambiente de desenvolvimento:

```bash
npm run dev
```

5) Gerar build de produção:

```bash
npm run build
```

6) Iniciar aplicação em modo produção:

```bash
npm run start
```

## Estrutura de pastas
```text
app/          # Rotas e páginas (App Router), layouts e metadados
components/   # Componentes de interface reutilizáveis
content/      # Conteúdo textual e dados de negócio (ex.: lista de serviços)
public/       # Arquivos estáticos (imagens, ícones, documentos)
```

## Editando conteúdo
Para alterações por pessoas sem conhecimento técnico:

- Atualize textos institucionais em **`content/`** (ex.: conteúdo de Home, Sobre e Contato).
- Atualize a lista de serviços também em **`content/`**.
- Evite editar arquivos em **`components/`** para mudanças de conteúdo.

> Diretriz: sempre priorizar alteração em dados/textos de `content/` e manter componentes apenas para estrutura visual.

## Scripts disponíveis
Sem `package.json` versionado neste repositório, considere apenas os scripts padrão de projeto Next.js.

| Comando | O que faz |
|---|---|
| `npm run dev` | Inicia o servidor de desenvolvimento |
| `npm run build` | Gera a build de produção |
| `npm run start` | Inicia a aplicação com a build de produção |
| `npm run lint` | Executa lint do projeto (`TODO`: confirmar se o script está habilitado no `package.json`) |

## Deploy
Fluxo esperado para deploy estático:

```bash
npm run build
```

Variáveis de ambiente em produção:
- Definir no provedor de deploy os mesmos nomes de `.env.example`.
- `TODO`: listar chaves obrigatórias quando o arquivo de ambiente estiver disponível.

## Convenções
- Commits no padrão **Conventional Commits**.
- Branches de trabalho criadas a partir de **`main`**.
- Executar lint e formatação antes de cada commit.
  - `TODO`: confirmar comando de formatação oficial do repositório.

## Contato
- Site: https://axolutions.com.br
- WhatsApp: (11) 94936-0561
- E-mail: contato@axolutions.com.br
