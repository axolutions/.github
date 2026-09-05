# Site institucional da Axolutions
Repositório do site institucional da Axolutions, com conteúdo e estrutura para publicação estática.

## Sobre
A Axolutions é uma startup brasileira de desenvolvimento de software, sediada em São Paulo (CNPJ 60.140.588/0001-00).

A empresa desenvolve soluções sob medida, incluindo:
- sites institucionais;
- sistemas web;
- aplicativos;
- e-commerces;
- automações.

Diferencial operacional: o cliente recebe uma prévia funcional no mesmo dia, sem custo e sem compromisso.

## Stack
- Next.js 14 (App Router)
- TypeScript
- Tailwind CSS
- Deploy estático
- Node.js: **>= 18.17.0**
- Gerenciador de pacotes: **TODO (não definido neste repositório)**

## Rodando localmente
1. Clone o repositório:

```bash
git clone <URL_DO_REPOSITORIO>
cd .github
```

2. Instale as dependências:

```bash
npm install
```

3. Configure variáveis de ambiente com base no arquivo `.env.example`:

```bash
cp .env.example .env.local
```

> TODO: criar/validar `.env.example` neste repositório, se ainda não existir.

4. Execute em modo de desenvolvimento:

```bash
npm run dev
```

5. Gere a build de produção:

```bash
npm run build
```

6. Inicie em modo produção:

```bash
npm run start
```

## Estrutura de pastas
```text
app/         # Rotas e páginas (App Router), layouts e composição principal da aplicação
components/  # Componentes de interface reutilizáveis
content/     # Conteúdo textual/estruturado das páginas (ex.: serviços, textos institucionais)
public/      # Arquivos estáticos servidos diretamente (imagens, ícones, etc.)
```

## Editando conteúdo
Para alterações sem mexer em componentes de UI:
- textos das páginas: editar os arquivos em `content/`;
- lista de serviços: editar a estrutura correspondente em `content/`.

Fluxo recomendado:
1. localizar o arquivo de conteúdo;
2. alterar apenas os dados/textos;
3. validar visualmente com o ambiente local (`npm run dev`).

## Scripts disponíveis
> Como não há `package.json` neste repositório, a tabela abaixo usa apenas scripts padrão de projetos Next.js.

| Comando | Função |
|---|---|
| `npm run dev` | Inicia o servidor de desenvolvimento |
| `npm run build` | Gera a build de produção |
| `npm run start` | Inicia a aplicação em modo produção |
| `TODO` | Confirmar scripts de lint/formatação quando definidos no `package.json` |

## Deploy
Deploy esperado: build estático de aplicação Next.js.

Passos base:

```bash
npm run build
```

> TODO: confirmar/exportar estratégia estática final (ex.: `output: "export"`) conforme configuração do projeto.

Variáveis de ambiente em produção:
- utilizar as mesmas chaves documentadas em `.env.example`.
- TODO: definir lista final de variáveis obrigatórias se ainda não estiver documentada.

## Convenções
- Commits no padrão **Conventional Commits**.
- Criação de branches a partir de `main`.
- Executar lint e formatação antes de commitar.
  - TODO: definir comandos oficiais de lint/formatação no `package.json`.

## Contato
- Site: https://axolutions.com.br
- WhatsApp: (11) 94936-0561
- E-mail: contato@axolutions.com.br
