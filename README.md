## 🏦 Sistema Bancário em Python

Este projeto implementa um sistema bancário simples em Python desenvolvido durante o Bootcamp Santander - Trilha Pyhton com a DIO, utilizando princípios de **Programação Orientada a Objetos (POO)**. Ele simula funcionalidades básicas de um banco como criação de usuários e contas, saques, depósitos e emissão de extratos.

---

### 📋 Funcionalidades

* Criar clientes (usuários).
* Criar contas bancárias para clientes.
* Realizar depósitos e saques.
* Consultar extrato de movimentações.
* Listar contas cadastradas.

---

### 🧠 Tecnologias e Conceitos Utilizados

* Python 3.x
* Programação Orientada a Objetos:

  * Herança
  * Encapsulamento
  * Abstração com `ABC`
  * Boas práticas com separação de responsabilidades:

  * Camada de modelo (`Cliente`, `Conta`, `Transacao`, etc.)
  * Camada de interface (menus e entradas)

---

### 🗂️ Estrutura do Projeto

```text
sistema_bancario/
├── main.py          # Arquivo principal com o loop do sistema
├── README.md        # Este arquivo
```

---

### ▶️ Como Executar

1. **Pré-requisitos:**

   * Python 3 instalado no sistema.

2. **Clonar ou baixar o repositório.**

3. **Executar:**

   ```bash
   python main.py
   ```

---

### 💻 Interface via Menu

Ao rodar o programa, um menu é exibido com as opções:

```text
=============== MENU ===============
[d]    Depositar
[s]    Sacar
[e]    Extrato
[nc]   Nova conta
[lc]   Listar contas
[nu]   Novo usuário
[q]    Sair
```

---

### 👤 Clientes e Contas

* Um cliente é identificado pelo **CPF** e pode ter múltiplas contas.
* Cada conta é uma instância da classe `ContaCorrente`.
* O cliente pode escolher com qual conta deseja operar.

---

### 📌 Regras de Negócio

* Limite de saque: **R\$ 500,00** por saque.
* Máximo de **3 saques por conta**.
* Depósitos e saques devem ter valores **positivos**.
* Extrato mostra todas as transações com **data e hora**.

---

### 🛠️ Possíveis Melhorias Futuras

* Armazenar dados em arquivos (`JSON`, `CSV`) ou banco de dados (`SQLite`, `MySQL`).
* Autenticação de usuários com senha.
