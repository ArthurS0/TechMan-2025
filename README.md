⚙️ Techman — Gestão de Manutenção de Equipamentos

📌 Sobre o projeto

O Techman é um sistema Full Stack desenvolvido para facilitar o controle e gerenciamento do histórico de manutenções de equipamentos.

O sistema permite que usuários autenticados visualizem equipamentos, consultem e adicionem comentários. Administradores possuem permissões extras para cadastrar e excluir equipamentos.

🛠️ Funcionalidades

🔑 Login com teclado virtual (6 dígitos)

📋 Listagem de equipamentos ativos

🖊️ Cadastro de novos equipamentos (admin)

🗑️ Exclusão de equipamentos (admin)

💬 Listagem e cadastro de comentários

👤 Perfis de usuário (admin / comum)

📂 Estrutura do Projeto
.
├── assets/              # Logotipo, ícones e ilustrações
├── dados/               # Arquivos CSV fornecidos
├── backend/             # API com Node.js, Express e Prisma
├── frontend/            # Aplicação Web (React/Vue/Angular ou HTML+CSS+JS)
├── diagramas/           # DER.png e DiagramaAtividades.png
├── script.sql           # Estrutura e importação do banco
└── README.md

🖼️ Diagramas

📊 DER (Diagrama Entidade-Relacionamento)

🔄 Diagrama de Atividades — Inclusão de Equipamento

🗄️ Banco de Dados

Banco: MySQL

ORM: Prisma

Estrutura baseada nos arquivos CSV fornecidos:

usuarios.csv

equipamentos.csv

comentarios.csv

perfis.csv

Importação dos dados

Via script.sql ou seed.js.

⚙️ Como rodar o projeto
🔹 Back-end
cd backend
npm install
# configure o arquivo .env
npx prisma migrate dev
node seed.js
npm run dev

🔹 Front-end
cd frontend
npm install
npm run dev


➡️ Acesse em: http://localhost:3000

👥 Perfis de Acesso

Administrador

Pode cadastrar e excluir equipamentos.

Pode visualizar e comentar.

Usuário comum

Pode visualizar equipamentos.

Pode visualizar e adicionar comentários.

🎨 Layout

Fonte: Trebuchet MS (12 pt títulos, 10 pt textos).

Paleta de cores: baseada no logotipo (em ./assets/).

Logotipo presente nas telas principais.

✅ Entregas

✔️ diagramas/DER.png
✔️ diagramas/DiagramaAtividades.png
✔️ script.sql
✔️ Código fonte backend/ + frontend/

🚀 Conclusão

O Techman é uma solução prática para o gerenciamento de equipamentos, oferecendo:

Login seguro,

Perfis de usuário,

Gestão de equipamentos,

Histórico de comentários.