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
Retornar status `401 Unauthorized`.

**Resultado obtido:**
Status `401 Unauthorized`.

**Status:** ✅ Aprovado

### Evidência

<img src="../evidencias/login/CT-LOGIN-002.jpeg" width="850">

---

# 2. Funcionários

## CT-FUNC-001 - Cadastro de funcionário

...

### Evidência

<img src="../evidencias/funcionarios/CT-FUNC-001.jpeg" width="850">

---

## CT-FUNC-002 - Listagem de funcionários

...

### Evidência

<img src="../evidencias/funcionarios/CT-FUNC-002.jpeg" width="850">

---

## CT-FUNC-003 - Atualização de funcionário

...

### Evidência

<img src="../evidencias/funcionarios/CT-FUNC-003.jpeg" width="850">

---

# 3. Motoristas

## CT-MOT-001 - Cadastro de motorista

...

### Evidência

<img src="../evidencias/motoristas/CT-MOT-001.jpeg" width="850">

---

## CT-MOT-002 - Listagem de motoristas

...

### Evidência

<img src="../evidencias/motoristas/CT-MOT-002.jpeg" width="850">

---

## CT-MOT-003 - Cadastro com prontuário duplicado

...

### Evidência

<img src="../evidencias/motoristas/CT-MOT-003.jpeg" width="850">

---

# 4. Veículos

## CT-VEI-001 - Cadastro de veículo

...

### Evidência

<img src="../evidencias/veiculos/CT-VEI-001.jpeg" width="850">

---

## CT-VEI-002 - Listagem de veículos

...

### Evidência

<img src="../evidencias/veiculos/CT-VEI-002.jpeg" width="850">

---

## CT-VEI-003 - Cadastro com placa duplicada

...

### Evidência

<img src="../evidencias/veiculos/CT-VEI-003.jpeg" width="850">

---

# 5. Corridas

## CT-COR-001 - Criação de solicitação de corrida

...

### Evidência

<img src="../evidencias/corridas/CT-COR-001.jpeg" width="850">

---

# Considerações Finais

Os casos de teste documentados neste arquivo representam a execução manual dos principais fluxos da API do sistema EMoov.

As evidências foram registradas por meio do Thunder Client e organizadas por módulo no repositório.
