# Casos de Teste - EMoov

Este documento apresenta os casos de teste manuais executados na API do sistema EMoov utilizando o Thunder Client.

---

## Resumo dos Testes

| Módulo | Quantidade |
|---|---:|
| Login | 2 |
| Funcionários | 3 |
| Motoristas | 3 |
| Veículos | 3 |
| Corridas | 1 |
| **Total** | **12** |

---

# 1. Login

## CT-LOGIN-001 - Login com credenciais válidas

**Objetivo:** Validar que o sistema permite autenticação com usuário e senha corretos.

**Método:** POST  
**Endpoint:** `/auth/login`

**Resultado esperado:**  
Retornar status `200 OK` e token de autenticação.

**Resultado obtido:**  
Status `200 OK` e token retornado com sucesso.

**Status:** Aprovado

**Evidência:**  
`evidencias/login/CT-LOGIN-001.png`

---

## CT-LOGIN-002 - Login com senha inválida

**Objetivo:** Validar que o sistema não permite autenticação com senha incorreta.

**Método:** POST  
**Endpoint:** `/auth/login`

**Resultado esperado:**  
Retornar status `401 Unauthorized`.

**Resultado obtido:**  
Status `401 Unauthorized`.

**Status:** Aprovado

**Evidência:**  
`evidencias/login/CT-LOGIN-002.png`

---

# 2. Funcionários

## CT-FUNC-001 - Cadastro de funcionário

**Objetivo:** Validar o cadastro de um funcionário com dados válidos.

**Método:** POST  
**Endpoint:** `/funcionario`

**Resultado esperado:**  
Funcionário cadastrado com sucesso.

**Resultado obtido:**  
Funcionário cadastrado com sucesso.

**Status:** Aprovado

**Evidência:**  
`evidencias/funcionarios/CT-FUNC-001.png`

---

## CT-FUNC-002 - Listagem de funcionários

**Objetivo:** Validar a listagem dos funcionários cadastrados.

**Método:** GET  
**Endpoint:** `/funcionario`

**Resultado esperado:**  
Retornar a lista de funcionários.

**Resultado obtido:**  
Lista de funcionários retornada com sucesso.

**Status:** Aprovado

**Evidência:**  
`evidencias/funcionarios/CT-FUNC-002.png`

---

## CT-FUNC-003 - Atualização de funcionário

**Objetivo:** Validar a atualização dos dados de um funcionário existente.

**Método:** PUT  
**Endpoint:** `/funcionario/{id}`

**Resultado esperado:**  
Funcionário atualizado com sucesso.

**Resultado obtido:**  
Funcionário atualizado com sucesso.

**Status:** Aprovado

**Evidência:**  
`evidencias/funcionarios/CT-FUNC-003.png`

---

# 3. Motoristas

## CT-MOT-001 - Cadastro de motorista

**Objetivo:** Validar o cadastro de um motorista com dados válidos.

**Método:** POST  
**Endpoint:** `/motorista`

**Resultado esperado:**  
Motorista cadastrado com sucesso.

**Resultado obtido:**  
Motorista cadastrado com sucesso.

**Status:** Aprovado

**Evidência:**  
`evidencias/motoristas/CT-MOT-001.png`

---

## CT-MOT-002 - Listagem de motoristas

**Objetivo:** Validar a listagem dos motoristas cadastrados.

**Método:** GET  
**Endpoint:** `/motorista`

**Resultado esperado:**  
Retornar a lista de motoristas.

**Resultado obtido:**  
Lista de motoristas retornada com sucesso.

**Status:** Aprovado

**Evidência:**  
`evidencias/motoristas/CT-MOT-002.png`

---

## CT-MOT-003 - Cadastro com prontuário duplicado

**Objetivo:** Validar que o sistema não permite cadastrar motorista com prontuário já existente.

**Método:** POST  
**Endpoint:** `/motorista`

**Resultado esperado:**  
Retornar erro informando duplicidade ou impedir o cadastro.

**Resultado obtido:**  
Cadastro não realizado devido ao prontuário duplicado.

**Status:** Aprovado

**Evidência:**  
`evidencias/motoristas/CT-MOT-003.png`

---

# 4. Veículos

## CT-VEI-001 - Cadastro de veículo

**Objetivo:** Validar o cadastro de um veículo com dados válidos.

**Método:** POST  
**Endpoint:** `/veiculo`

**Resultado esperado:**  
Veículo cadastrado com sucesso.

**Resultado obtido:**  
Veículo cadastrado com sucesso.

**Status:** Aprovado

**Evidência:**  
`evidencias/veiculos/CT-VEI-001.png`

---

## CT-VEI-002 - Listagem de veículos

**Objetivo:** Validar a listagem dos veículos cadastrados.

**Método:** GET  
**Endpoint:** `/veiculo`

**Resultado esperado:**  
Retornar a lista de veículos.

**Resultado obtido:**  
Lista de veículos retornada com sucesso.

**Status:** Aprovado

**Evidência:**  
`evidencias/veiculos/CT-VEI-002.png`

---

## CT-VEI-003 - Cadastro com placa duplicada

**Objetivo:** Validar que o sistema não permite cadastrar veículo com placa já existente.

**Método:** POST  
**Endpoint:** `/veiculo`

**Resultado esperado:**  
Retornar erro informando duplicidade ou impedir o cadastro.

**Resultado obtido:**  
Cadastro não realizado devido à placa duplicada.

**Status:** Aprovado

**Evidência:**  
`evidencias/veiculos/CT-VEI-003.png`

---

# 5. Corridas

## CT-COR-001 - Criação de solicitação de corrida

**Objetivo:** Validar a criação de uma solicitação de corrida com dados válidos.

**Método:** POST  
**Endpoint:** `/corridas`

**Resultado esperado:**  
Corrida criada com sucesso.

**Resultado obtido:**  
Corrida criada com sucesso.

**Status:** Aprovado

**Evidência:**  
`evidencias/corridas/CT-COR-001.png`

---

# Considerações Finais

Os casos de teste documentados neste arquivo representam a execução manual dos principais fluxos da API do sistema EMoov.

As evidências foram registradas por meio do Thunder Client e organizadas por módulo no repositório.
