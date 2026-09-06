**1. Conteúdo do Arquivo `README.md**`

```markdown
# Solução — Sistema de Gestão e Controle de Estoque de Doações

## 🐾 Sobre o Projeto
O **Solução** é um sistema web desenvolvido para a ONG **Amigos de Quatro Patas**, localizada em Assis-SP. A instituição resgata, reabilita e promove a doação de animais em situação de abandono e maus-tratos.

O objetivo é eliminar o descontrole no estoque de doações (rações, medicamentos e insumos), permitindo registros centralizados, controle de validade e alertas visuais automáticos para itens com estoque mínimo.

---

## 📁 Estrutura do Repositório
```text
solucao-estoque-ong/
├── docs/        # Documentação e Documento de Visão (PDF)
├── database/    # Scripts SQL para criação das tabelas
├── backend/     # API REST (Node.js + Express)
├── frontend/    # Interface Web (React.js)
├── .env.example # Exemplo de variáveis de ambiente
└── .gitignore   # Arquivos ignorados pelo Git

```

---

## 🛠️ Instruções de Instalação e Execução Local

### Pré-requisitos

* **Node.js** (versão 18 ou superior)
* **Git** instalado

### Passo a Passo

1. **Clonar o repositório:**
```bash
git clone [https://github.com/SEU_USUARIO/solucao-estoque-ong.git](https://github.com/SEU_USUARIO/solucao-estoque-ong.git)
cd solucao-estoque-ong

```


2. **Configurar o Backend:**
```bash
cd backend
npm install
cp ../.env.example .env
npm run dev

```


3. **Configurar o Frontend:**
```bash
cd ../frontend
npm install
npm start

```



---

## 👨‍💻 Autor

* **Aluno:** Pedro Henrique de Paiva
* **Disciplina:** Projeto Integrador Extensionista I - PIE I
* **Data:** 31/08/2026

```

---

**2. Conteúdo do Arquivo `.env.example`**

```env
# Servidor Backend
PORT=3000
NODE_ENV=development

# Conexão Banco de Dados
DB_HOST=localhost
DB_PORT=5432
DB_USER=seu_usuario
DB_PASS=sua_senha
DB_NAME=estoque_ong

# Autenticação JWT
JWT_SECRET=sua_chave_secreta_jwt

```

---

**3. Conteúdo do Arquivo `.gitignore**`

```text
node_modules/
.env
.env.local
dist/
build/
*.log
.DS_Store
Thumbs.db

```

---

**4. Como Registrar os 3 Commits Exigidos**

Caso utilize o **Git Bash** ou o **Terminal** da sua máquina, execute os seguintes comandos em ordem na pasta do projeto:

* **Commit 1 (Estrutura e Configurações):**
```bash
git add .gitignore .env.example database/
git commit -m "chore: estrutura inicial do repositorio, pastas do projeto e .env.example"

```


* **Commit 2 (Documento de Visão):**
```bash
git add docs/
git commit -m "docs: adiciona o Documento de Visao em PDF na pasta docs"

```


* **Commit 3 (README e Aplicação):**
```bash
git add README.md backend/ frontend/
git commit -m "docs: adiciona README com instrucoes de instalacao e arquivos base"

```



