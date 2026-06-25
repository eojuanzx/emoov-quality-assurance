# Casos de Teste - EMoov

Este documento apresenta os casos de teste manuais executados na API do sistema EMoov utilizando o Thunder Client.

---

## Resumo dos Testes

| Módulo       | Quantidade |
| ------------ | ---------: |
| Login        |          2 |
| Funcionários |          3 |
| Motoristas   |          3 |
| Veículos     |          3 |
| Corridas     |          1 |
| **Total**    |     **12** |

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

**Status:** ✅ Aprovado

### Evidência

<img src="../evidencias/login/CT-LOGIN-001.jpeg" width="850">

---

## CT-LOGIN-002 - Login com senha inválida

**Objetivo:** Validar que o sistema não permite autenticação com senha incorreta.

**Método:** POST  
**Endpoint:** `/auth/login`

**Resultado esperado:**  
Retornar status `401 Unauthorized` e mensagem de erro informando credenciais inválidas.

**Resultado obtido:**  
Status `401 Unauthorized` retornado corretamente.

**Status:** ✅ Aprovado

### Evidência

<img src="../evidencias/login/CT-LOGIN-002.jpeg" width="850">

---

# 2. Funcionários

## CT-FUNC-001 - Cadastro de funcionário

**Objetivo:** Validar o cadastro de um funcionário com dados válidos.

**Método:** POST  
**Endpoint:** `/funcionario`

**Resultado esperado:**  
Retornar status de sucesso e cadastrar o funcionário corretamente.

**Resultado obtido:**  
Funcionário cadastrado com sucesso.

**Status:** ✅ Aprovado

### Evidência

<img src="../evidencias/funcionarios/CT-FUNC-001.jpeg" width="850">

---

## CT-FUNC-002 - Listagem de funcionários

**Objetivo:** Validar a listagem dos funcionários cadastrados.

**Método:** GET  
**Endpoint:** `/funcionario`

**Resultado esperado:**  
Retornar status `200 OK` e a lista de funcionários cadastrados.

**Resultado obtido:**  
Lista de funcionários retornada com sucesso.

**Status:** ✅ Aprovado

### Evidência

<img src="../evidencias/funcionarios/CT-FUNC-002.jpeg" width="850">

---

## CT-FUNC-003 - Atualização de funcionário

**Objetivo:** Validar a atualização dos dados de um funcionário existente.

**Método:** PUT  
**Endpoint:** `/funcionario/{id}`

**Resultado esperado:**  
Retornar status de sucesso e atualizar os dados do funcionário.

**Resultado obtido:**  
Funcionário atualizado com sucesso.

**Status:** ✅ Aprovado

### Evidência

<img src="../evidencias/funcionarios/CT-FUNC-003.jpeg" width="850">

---

# 3. Motoristas

## CT-MOT-001 - Cadastro de motorista

**Objetivo:** Validar o cadastro de um motorista com dados válidos.

**Método:** POST  
**Endpoint:** `/motorista`

**Resultado esperado:**  
Retornar status de sucesso e cadastrar o motorista corretamente.

**Resultado obtido:**  
Motorista cadastrado com sucesso.

**Status:** ✅ Aprovado

### Evidência

<img src="../evidencias/motoristas/CT-MOT-001.jpeg" width="850">

---

## CT-MOT-002 - Listagem de motoristas

**Objetivo:** Validar a listagem dos motoristas cadastrados.

**Método:** GET  
**Endpoint:** `/motorista`

**Resultado esperado:**  
Retornar status `200 OK` e a lista de motoristas cadastrados.

**Resultado obtido:**  
Lista de motoristas retornada com sucesso.

**Status:** ✅ Aprovado

### Evidência

<img src="../evidencias/motoristas/CT-MOT-002.jpeg" width="850">

---

## CT-MOT-003 - Cadastro com prontuário duplicado

**Objetivo:** Validar que o sistema não permite cadastrar motorista com prontuário já existente.

**Método:** POST  
**Endpoint:** `/motorista`

**Resultado esperado:**  
Impedir o cadastro duplicado e retornar mensagem de erro.

**Resultado obtido:**  
Cadastro não realizado devido ao prontuário duplicado.

**Status:** ✅ Aprovado

### Evidência

<img src="../evidencias/motoristas/CT-MOT-003.jpeg" width="850">

---

# 4. Veículos

## CT-VEI-001 - Cadastro de veículo

**Objetivo:** Validar o cadastro de um veículo com dados válidos.

**Método:** POST  
**Endpoint:** `/veiculo`

**Resultado esperado:**  
Retornar status de sucesso e cadastrar o veículo corretamente.

**Resultado obtido:**  
Veículo cadastrado com sucesso.

**Status:** ✅ Aprovado

### Evidência

<img src="../evidencias/veiculos/CT-VEI-001.jpeg" width="850">

---

## CT-VEI-002 - Listagem de veículos

**Objetivo:** Validar a listagem dos veículos cadastrados.

**Método:** GET  
**Endpoint:** `/veiculo`

**Resultado esperado:**  
Retornar status `200 OK` e a lista de veículos cadastrados.

**Resultado obtido:**  
Lista de veículos retornada com sucesso.

**Status:** ✅ Aprovado

### Evidência

<img src="../evidencias/veiculos/CT-VEI-002.jpeg" width="850">

---

## CT-VEI-003 - Cadastro com placa duplicada

**Objetivo:** Validar que o sistema não permite cadastrar veículo com placa já existente.

**Método:** POST  
**Endpoint:** `/veiculo`

**Resultado esperado:**  
Impedir o cadastro duplicado e retornar mensagem de erro.

**Resultado obtido:**  
Cadastro não realizado devido à placa duplicada.

**Status:** ✅ Aprovado

### Evidência

<img src="../evidencias/veiculos/CT-VEI-003.jpeg" width="850">

---

# 5. Corridas

## CT-COR-001 - Criação de solicitação de corrida

**Objetivo:** Validar a criação de uma solicitação de corrida com dados válidos.

**Método:** POST  
**Endpoint:** `/corridas`

**Resultado esperado:**  
Retornar status de sucesso e criar a solicitação de corrida.

**Resultado obtido:**  
Corrida criada com sucesso.

**Status:** ✅ Aprovado

### Evidência

<img src="../evidencias/corridas/CT-COR-001.jpeg" width="850">

---

# Considerações Finais

Os casos de teste documentados neste arquivo representam a execução manual dos principais fluxos da API do sistema EMoov.

As evidências foram registradas por meio do Thunder Client e organizadas por módulo no repositório.
