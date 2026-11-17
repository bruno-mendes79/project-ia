# AGENTS.md

Diretrizes e convenções para agentes de IA que operam no repositório.

## Stack e Arquitetura

- **Framework:** Next.js (App Router) com Turbopack
- **UI:** React (Server Components por padrão)
- **Documentação Local:** A documentação completa da versão instalada do Next.js está acessível em `node_modules/next/dist/docs/`.
- **Dependências:** Consulte sempre o [package.json](file:///home/bruno/project-ia/package.json) para verificar as versões instaladas.

## Comandos Principais

- `npm run dev`: Inicia o servidor de desenvolvimento.
- `npm run build`: Executa o build de produção.
- `npm run start`: Inicia o servidor em produção.

## Diretrizes de Desenvolvimento

1. **Simplicidade e Minimalismo:**
   - Priorize soluções simples, limpas e com o mínimo de código necessário.
   - Evite adicionar novas dependências, abstrações ou complexidade sem necessidade clara.

2. **Convenções do Next.js:**
   - Adote sempre o **App Router** (`app/`).
   - Mantenha componentes como **React Server Components (RSC)** por padrão. Utilize `'use client'` apenas quando for estritamente necessário (estados locais, efeitos ou manipuladores de eventos do navegador).
   - Utilize a `metadata` API para gerenciamento de títulos e metadados de páginas e layouts.

3. **Estilização:**
   - Mantenha a estilização simples e direta, sem introduzir bibliotecas ou frameworks pesados sem solicitação explícita.

4. **Boas Práticas de Versionamento:**
   - Mantenha commits concisos e objetivos.
   - Garanta que artefatos de build e dependências (`.next`, `node_modules`) permaneçam ignorados.
