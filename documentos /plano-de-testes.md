# Plano de Testes - EMoov

## 1. Introdução

Este documento apresenta o plano de testes manuais realizado no sistema **EMoov**, uma plataforma de mobilidade interna e controle de frota desenvolvida como Trabalho de Conclusão de Curso.

O objetivo deste plano é definir o escopo, a estratégia, o ambiente, as funcionalidades testadas e os critérios utilizados durante a execução dos testes.

---

## 2. Objetivo dos Testes

Validar o funcionamento das principais funcionalidades do sistema EMoov, garantindo que os módulos essenciais estejam operando conforme o esperado.

Os testes têm como foco:

- Validar a autenticação de usuários por meio do endpoint de login;
- Validar o cadastro, a listagem e a atualização de funcionários;
- Validar o cadastro e a listagem de motoristas;
- Validar o cadastro e a listagem de veículos;
- Validar a criação de solicitações de corrida;
- Registrar evidências dos testes executados;
- Identificar comportamentos inesperados durante a validação da API.

---

## 3. Escopo dos Testes

### Funcionalidades testadas

- Login
- Cadastro de funcionários
- Listagem de funcionários
- Atualização de funcionários
- Cadastro de motoristas
- Listagem de motoristas
- Validação de duplicidade de prontuário de motorista
- Cadastro de veículos
- Listagem de veículos
- Validação de duplicidade de placa de veículo
- Criação de solicitação de corrida

### Fora do escopo

- Testes automatizados
- Testes de performance
- Testes de carga
- Testes de segurança avançados
- Testes de usabilidade completos
- Testes automatizados de interface
- Validação completa dos fluxos via WebSocket

---

## 4. Estratégia de Testes

Foram realizados **testes manuais funcionais** com foco na validação da API REST do sistema.

A execução dos testes foi feita por meio do **Thunder Client**, simulando requisições HTTP para os principais endpoints do backend.

Foram considerados cenários positivos e negativos, como:

- Cadastro com dados válidos;
- Listagem de registros;
- Atualização de dados;
- Tentativa de cadastro com prontuário já existente;
- Tentativa de cadastro com placa já cadastrada;
- Login válido;
- Login inválido;
- Criação de solicitação de corrida.

---

## 5. Ambiente de Testes

| Item | Descrição |
|---|---|
| Sistema testado | EMoov |
| Tipo de teste | Teste manual funcional |
| Ferramenta de teste | Thunder Client |
| Backend | NestJS |
| Banco de dados | PostgreSQL / Supabase |
| ORM | Prisma |
| Autenticação | JWT |
| Ambiente | Local |
| URL base | `http://localhost:3000` |

---

## 6. Módulos Testados

| Módulo | Tipo de validação |
|---|---|
| Login | Autenticação e retorno de token |
| Funcionários | Cadastro, listagem e atualização |
| Motoristas | Cadastro, listagem e validação de duplicidade |
| Veículos | Cadastro, listagem e validação de duplicidade |
| Corridas | Criação de solicitação de corrida |

---

## 7. Critérios de Entrada

Para iniciar os testes, foram considerados os seguintes critérios:

- Backend executando localmente;
- Banco de dados conectado;
- Thunder Client instalado e configurado;
- Endpoints disponíveis para teste;
- Massa de dados mínima cadastrada;
- Usuário válido disponível para autenticação.

---

## 8. Critérios de Saída

Os testes foram considerados concluídos quando:

- Os principais módulos definidos no escopo foram testados;
- As evidências foram registradas;
- Os resultados obtidos foram comparados com os resultados esperados;
- Os casos de teste foram documentados;
- As falhas encontradas foram identificadas para possível correção futura.

---

## 9. Tipos de Teste Realizados

- Testes funcionais;
- Testes de API REST;
- Testes positivos;
- Testes negativos;
- Testes de validação de dados;
- Testes de validação de regras de negócio.

---

## 10. Evidências

As evidências dos testes foram registradas por meio de capturas de tela das requisições executadas no **Thunder Client**, permitindo documentar as entradas enviadas, as respostas obtidas e os códigos de status retornados pela API.

As evidências foram organizadas por módulo para facilitar a consulta e a rastreabilidade dos testes realizados.

```text
evidencias/
├── login/
├── funcionarios/
├── motoristas/
├── veiculos/
└── corridas/
```

Cada captura de tela está vinculada ao respectivo caso de teste documentado neste repositório, servindo como comprovação da execução e dos resultados obtidos.
