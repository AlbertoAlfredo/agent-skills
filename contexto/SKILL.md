---
name: gerar-contexto
description: Automatiza a criação e atualização do arquivo de contexto do projeto (CONTEXT.md)
license: MIT
compatibility: opencode
---

# Automação de Contexto do Projeto
Sempre que o usuário solicitar a atualização ou criação do contexto, siga rigidamente estes passos:

1. **Escanear Diretórios**: Liste a árvore de arquivos principais para entender a arquitetura atual (ignore `node_modules`, `dist`, `.git`).
2. **Identificar Tecnologias**: Verifique arquivos como `package.json`, `requirements.txt` ou `go.mod` para listar o ecossistema técnico.
3. **Gerar/Atualizar CONTEXT.md**: Crie ou sobrescreva o arquivo `CONTEXT.md` na raiz do projeto com a estrutura abaixo:

```markdown
# Contexto do Projeto: [Nome do Projeto]

## 🎯 Objetivo
- [Breve descrição do propósito do software]

## 🛠️ Stack Tecnológica
- **Linguagem/Framework**: [Ex: Next.js, Python FastApi]
- **Banco de Dados**: [Ex: PostgreSQL]
- **Estilização/Ferramentas**: [Ex: Tailwind CSS]

## 📂 Estrutura de Arquivos Principal
- [Listar principais pastas e arquivos estratégicos com uma breve explicação]

## 🚀 Estado Atual & Próximos Passos
- [O que já está funcionando]
- [O que precisa ser feito a seguir]
```

4. **Confirmação**: Informe ao usuário que o `CONTEXT.md` foi gerado com sucesso e liste as seções atualizadas.
