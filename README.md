# 🩺 Doutor Agenda

![Status](https://img.shields.io/badge/status-Em%20Desenvolvimento-blueviolet?style=for-the-badge)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-38B2AC?style=for-the-badge&logo=tailwindcss&logoColor=white)
![ESLint](https://img.shields.io/badge/ESLint-4B32C3?style=for-the-badge&logo=eslint&logoColor=white)
![License](https://img.shields.io/github/license/vivianedev/doutor-agenda?style=for-the-badge)

> Sistema de agendamento de consultas para clínicas, com autenticação, gestão de médicos e pacientes, planos e agendamentos.

---

## 🚀 Tecnologias Utilizadas

<p align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" width="40" alt="TypeScript"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nextjs/nextjs-original.svg" width="40" alt="Next.js"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tailwindcss/tailwindcss-plain.svg" width="40" alt="TailwindCSS"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/eslint/eslint-original.svg" width="40" alt="ESLint"/>
</p>

---

## 📋 Funcionalidades

- 🔐 Autenticação de usuários
- 🏥 Gestão de clínicas (usuários múltiplos por clínica)
- 👨‍⚕️ CRUD de médicos
- 👥 Cadastro de pacientes
- 📅 Agendamentos médico ↔ paciente
- 💳 Planos de assinatura com controle de preços

---

## 🧠 Modelagem de dados (PostgreSQL)

- 👤 **User ↔ Clinic** (N:N)
- 🏥 **Clinic → Doctors / Patients / Appointments** (1:N)
- 👨‍⚕️ **Doctor → Appointments** (1:N)
- 🧑‍🤝‍🧑 **Patient → Appointments** (1:N)

> Ver `docs/erd.png` para visualização do modelo.

---

## 📦 Estrutura Inicial

```
doutor-agenda/
├── apps/
│   ├── web/           # Frontend Next.js
│   └── api/           # Backend NestJS
├── packages/
│   └── config/        # Shared configs (eslintrc, prettier, tsconfig, etc)
├── prisma/            # Migrações e seed
├── .vscode/
├── .eslintrc.js
├── tailwind.config.js
├── tsconfig.json
└── package.json
```

---

## ▶️ Como executar

```bash
# Clone o projeto
git clone https://github.com/vivianedev/doutor-agenda.git

# Acesse o diretório
cd doutor-agenda

# Instale as dependências
npm install

# Rode a aplicação em modo desenvolvimento
npm run dev
```

> Obs.: verifique se o PostgreSQL está instalado e rodando em sua máquina.

---

## 📍 Roadmap

- [x] Estrutura inicial do projeto
- [ ] Setup do banco com Drizzle
- [ ] Autenticação e cadastro de usuários
- [ ] CRUD de clínicas, médicos e pacientes
- [ ] Agendamento de consultas
- [ ] Integração com planos de assinatura
- [ ] Testes automatizados

---

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma [issue](https://github.com/vivianedev/doutor-agenda/issues) ou enviar um PR.

---

## 📄 Licença

Distribuído sob a licença MIT. Veja `LICENSE` para mais informações.
