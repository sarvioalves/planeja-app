# 💻 Planeja App — Front-end de Gestão Financeira

Interface web moderna desenvolvida em **Angular 21** para planejamento e controle financeiro pessoal. A aplicação permite o gerenciamento completo de cartões de crédito, categorias de despesas/receitas e lançamentos financeiros, consumindo uma API REST própria.

> 🔗 **Repositório Back-end:** Para que todas as funcionalidades operem completamente, é necessário rodar a API em Java/Spring Boot. Confira o código do servidor aqui: **[Planeja API](https://github.com/sarvioalves/planeja-api-server)**

---

## 🚀 Funcionalidades

- **Gestão de Cartões:** Formulário de cadastro e tela de listagem de cartões de crédito/débito.
- **Gestão de Categorias:** Criação e organização visual de categorias para receitas e despesas.
- **Controle de Lançamentos:** Registro e acompanhamento detalhado de movimentações financeiras.
- **Arquitetura Modular:** Separação clara entre serviços de comunicação HTTP, componentes compartilhados e layout base.

---

## 🛠️ Tecnologias Utilizadas

* **[Angular 21](https://angular.dev)** — Framework principal (Single Page Application)
* **[TypeScript](https://typescriptlang.org)** — Superset JavaScript com tipagem estática
* **HTML5 & CSS3** — Estruturação semântica e estilização das telas
* **[Vitest](https://vitest.dev)** — Framework de testes unitários configurado no projeto
* **[Prettier](https://prettier.io) & EditorConfig** — Padronização e formatação de código

---

## 📂 Estrutura de Diretórios

A organização do repositório segue a arquitetura padrão do Angular CLI 21, dividida por domínios funcionais dentro de `src/app/`:

```text
planeja-app/
├── public/                     # Ativos estáticos públicos
├── src/
│   ├── app/
│   │   ├── cartoes/            # Cadastro, listagem e serviço de cartões
│   │   ├── categorias/         # Cadastro, listagem e serviço de categorias
│   │   ├── lancamentos/        # Cadastro, listagem e serviço de lançamentos
│   │   ├── common/components/  # Componentes reutilizáveis (Header)
│   │   └── template/           # Estrutura e layout base da aplicação
│   ├── index.html              # Página HTML principal
│   └── main.ts                 # Ponto de entrada da aplicação Angular
├── angular.json                # Configurações do workspace e build Angular
├── package.json                # Dependências e scripts do projeto
└── tsconfig.json               # Configurações do compilador TypeScript
```

---

## ⚙️ Como Executar o Projeto Localmente

### Pré-requisitos
* **[Node.js](https://nodejs.org)** (versão LTS recomendada) e **npm** instalados
* **[Angular CLI](https://angular.devtools/cli)** instalado globalmente (`npm install -g @angular/cli`)
* **Back-end (`planeja-api`)** em execução na porta `8080`

### Passo a passo

1. **Clone o repositório:**
   ```bash
   git clone https://github.com
   ```

2. **Acesse a pasta do projeto:**
   ```bash
   cd planeja-app
   ```

3. **Instale as dependências:**
   ```bash
   npm install
   ```

4. **Inicie o servidor de desenvolvimento:**
   ```bash
   ng serve
   ```

5. Abra o navegador e acesse `http://localhost:4200/`. A aplicação recarregará automaticamente se você alterar qualquer arquivo.

---

## 🧪 Executando os Testes e Build

* **Rodar testes unitários (Vitest):**
  ```bash
  ng test
  ```
* **Gerar build de produção (pasta `dist/`):**
  ```bash
  ng build
  ```

---

## 📸 Demonstração


![Preview do Planeja App](.public\demonstracao.png)

---

## 👨‍💻 Autor

Desenvolvido por **Sárvio Alves**.

Este projeto foi desenvolvido durante o treinamento **Angular 21 e Spring Boot 4 Completo**, com o objetivo de aplicar na prática a construção de interfaces modernas e reativas em **Single Page Applications (SPA)** integradas a uma API REST.

Durante o desenvolvimento, foram praticados conceitos como:
- Arquitetura modular e componentização no Angular 21;
- Consumo de serviços HTTP e integração com back-end Java;
- Tipagem estática com TypeScript e organização de fluxos de cadastro e listagem;
- Padronização de código e testes unitários com Vitest.
