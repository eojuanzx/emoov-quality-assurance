# Ambiente de Testes - EMoov

## Objetivo

Este documento descreve o ambiente utilizado para a execução dos testes manuais da API do sistema **EMoov**.

---

## Sistema Testado

**Nome:** EMoov  
**Tipo:** Sistema de mobilidade interna e controle de frota  
**Camada testada:** API REST / Backend

---

## Ambiente de Execução

| Item | Descrição |
|---|---|
| Ambiente | Local |
| URL Base | `http://localhost:3000` |
| Sistema Operacional | Windows |
| Ferramenta de Teste | Thunder Client |
| IDE utilizada | Visual Studio Code |
| Tipo de teste | Teste manual funcional |

---

## Tecnologias do Sistema

| Tecnologia | Utilização |
|---|---|
| NestJS | Backend da aplicação |
| TypeScript | Linguagem utilizada no backend |
| Prisma ORM | Comunicação com o banco de dados |
| PostgreSQL | Banco de dados |
| Supabase | Hospedagem/gerenciamento do banco PostgreSQL |
| JWT | Autenticação |
| Socket.IO | Comunicação em tempo real |

---

## Módulos Validados

Durante a execução dos testes, foram validados os seguintes módulos da API:

- Login
- Funcionários
- Motoristas
- Veículos
- Corridas

---

## Ferramenta de Testes

Os testes foram executados manualmente utilizando o **Thunder Client**, extensão do Visual Studio Code voltada para testes de APIs REST.

A ferramenta foi utilizada para:

- Enviar requisições HTTP;
- Validar códigos de status;
- Conferir respostas da API;
- Registrar evidências dos testes executados.

---

## Observações

Os testes foram realizados em ambiente local, com o backend em execução na máquina do desenvolvedor.

Não foram realizados testes automatizados, testes de carga, testes de performance ou testes de segurança nesta etapa.
