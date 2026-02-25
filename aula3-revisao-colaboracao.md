# Guia de Trabalho e Colaboração no GitHub

Este documento apresenta um guia completo sobre o fluxo de trabalho (**Workflow**), as formas de colaboração e as boas práticas para manter um repositório organizado e profissional.

---

## 1. O Ciclo de Trabalho (GitHub Flow)

O GitHub Flow é um fluxo de trabalho leve e focado em ramos (branches) que suporta equipes e projetos que realizam entregas contínuas.

1.  **Main Branch:** O branch `main` (ou `master`) contém sempre o código em estado de produção (estável).
2.  **Criação de Branches:** Nunca trabalhe diretamente na `main`. Crie uma branch secundária para cada nova funcionalidade ou correção:
    * Exemplo: `feature/adicionar-login` ou `bugfix/correcao-header`.
3.  **Commits:** Realize commits locais conforme avança no trabalho.
4.  **Pull Request (PR):** Quando o trabalho estiver pronto (ou precisar de feedback), abra um Pull Request para fundir sua branch com a `main`.
5.  **Code Review:** Outros colaboradores revisam o código, fazem comentários e sugerem alterações.
6.  **Merge:** Após a aprovação, o código é mesclado à branch principal e a branch auxiliar é deletada.

---

## 2. Formas de Colaboração

Existem duas formas principais de contribuir para um projeto no GitHub:

### A. Modelo de Repositório Compartilhado
Comum em equipes pequenas ou empresas. Os colaboradores têm permissão de escrita direta no repositório.
* Você clona o repositório.
* Cria uma branch.
* Envia o "Push" direto para o repositório original.

### B. Modelo Fork & Pull
Padrão em projetos **Open Source**. Você não tem permissão de escrita no repositório original.
1.  **Fork:** Você cria uma cópia do repositório original na sua conta.
2.  **Clone:** Baixa a sua cópia para sua máquina.
3.  **Push:** Envia as alterações para o *seu* fork.
4.  **Pull Request:** Solicita ao dono do repositório original que aceite suas melhorias.

---

## 3. Boas Práticas Essenciais

### 📝 Mensagens de Commit
Use o padrão de **Conventional Commits** para manter o histórico legível:
* `feat:` para novas funcionalidades.
* `fix:` para correção de bugs.
* `docs:` para mudanças na documentação.
* `style:` para formatação (espaços, vírgulas) que não afeta o código.

**Exemplo:** `git commit -m "feat: adiciona validação de e-mail no formulário"`

### 🌿 Gestão de Branches
* Mantenha suas branches atualizadas com a `main` para evitar conflitos (`git pull origin main`).
* Dê nomes descritivos e use hifens: `nome-da-branch`.
* Delete a branch logo após o merge bem-sucedido.

### 🔍 Pull Requests de Qualidade
* **Descrição clara:** Explique *o que* foi feito e *por que*.
* **Screenshots:** Se for uma alteração visual (UI), anexe imagens ou GIFs.
* **Checklist:** Inclua uma lista de tarefas confirmando que os testes foram feitos.

---

## 4. Comandos Essenciais (Cheat Sheet)

| Comando | Descrição |
| :--- | :--- |
| `git clone <url>` | Baixa o repositório para sua máquina. |
| `git checkout -b <nome>` | Cria e entra em uma nova branch. |
| `git add .` | Prepara todos os arquivos alterados. |
| `git commit -m "msg"` | Grava as alterações com uma mensagem. |
| `git push origin <branch>` | Envia as alterações para o GitHub. |
| `git pull origin main` | Atualiza seu código local com a versão mais recente. |

---

## 5. O Arquivo .gitignore
Sempre utilize um arquivo `.gitignore` para evitar o envio de arquivos desnecessários ao repositório, como:
* Pastas de dependências (`node_modules`).
* Arquivos de configuração local (`.env`).
* Arquivos temporários do sistema operacional (`.DS_Store`).

---
*Guia criado para padronização de fluxos de desenvolvimento.*