# Guia: Criando Páginas Estáticas com GitHub Pages

O **GitHub Pages** é um serviço de hospedagem de sites estáticos que extrai arquivos HTML, CSS e JavaScript diretamente de um repositório no GitHub e publica o site na web.

---

## O que é um Site Estático?

Diferente de sites dinâmicos (como WordPress ou sistemas que dependem de bancos de dados ativos em tempo de execução), um **site estático** entrega ao navegador exatamente o que está armazenado no servidor. 

### Benefícios:
* **Velocidade:** Carregamento quase instantâneo.
* **Segurança:** Sem banco de dados para invadir.
* **Custo Zero:** Hospedagem gratuita para repositórios públicos.
* **Certificado SSL:** HTTPS nativo e automático.

---

## Como Criar sua Página Estática

Existem duas formas principais de ativar o GitHub Pages:

### 1. Usando um Repositório Especial (Site de Usuário)
Ideal para seu portfólio pessoal ou currículo.
1. Crie um novo repositório com o nome: `seunome.github.io` (substitua "seunome" pelo seu login).
2. Suba seu arquivo `index.html` para o branch principal (`main`).
3. O site estará disponível em: `https://seunome.github.io`.

### 2. Usando um Repositório de Projeto
Ideal para documentação ou sites de projetos específicos.
1. Vá até as **Settings** (Configurações) do seu repositório.
2. No menu lateral esquerdo, clique em **Pages**.
3. Em **Build and deployment**, escolha o branch que deseja publicar (geralmente `main` ou `master`).
4. Clique em **Save**.

---

## Estrutura de Arquivos Recomendada

Para que o GitHub Pages identifique seu site, o arquivo principal deve estar na raiz do projeto:

```text
meu-projeto/
├── index.html       <-- Arquivo obrigatório na raiz
├── css/
│   └── style.css
├── js/
│   └── script.js
└── assets/
    └── logo.png