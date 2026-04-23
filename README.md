# 🧪 Automação de Testes E2E com BDD (Cucumber + Ruby)

## 📌 Sobre o projeto
Este projeto demonstra a automação de testes end-to-end (E2E) utilizando BDD (Behavior-Driven Development) com Cucumber.

Os cenários foram escritos em Gherkin, simulando o comportamento do usuário em uma aplicação web de e-commerce de cafés (Starbugs), validando fluxos de compra e regras de negócio.

---

## 🚀 Tecnologias utilizadas

- Cucumber
- Ruby
- Gherkin
- Capybara

---

## 🧪 Cenários testados

- Visualização do catálogo de produtos
- Início do fluxo de compra
- Validação de produto indisponível
- Aplicação de cupons de desconto
- Validação de cupons inválidos e expirados

---

## 🔍 Cenários de teste detalhados

### ☕ Catálogo de produtos

**Cenário: Acessar catálogo**
- Acessar página principal
- Validar exibição dos produtos disponíveis

**Cenário: Iniciar compra**
- Selecionar produto
- Validar redirecionamento para checkout
- Validar valor total da compra

**Cenário: Produto indisponível**
- Selecionar produto indisponível
- Validar exibição de mensagem de erro

---

### 💰 Aplicação de cupons

**Cenário: Cupom válido**
- Aplicar cupom "MEUCAFE"
- Validar desconto aplicado corretamente

**Cenário: Cupom inválido/expirado**
- Aplicar cupons inválidos
- Validar mensagens de erro exibidas

---

## 📸 Evidências dos testes

### 💰 Aplicação de cupom com sucesso

![Aplicação de cupom](logs/screenshots/4380.png)

Neste cenário, o cupom "MEUCAFE" foi aplicado com sucesso, resultando no cálculo correto do valor final da compra.

---

### ⚠️ Produto indisponível

![Produto indisponível](logs/screenshots/4360.png)

Neste cenário, o sistema apresenta corretamente uma mensagem de indisponibilidade ao tentar iniciar a compra de um produto fora de estoque.

---

## 📂 Estrutura do projeto

```
features/
├── catalogo.feature
├── cupom.feature
├── step_definitions/
├── support/
logs/
├── screenshots/
```

---

## ▶️ Como executar o projeto

### 1. Instalar dependências

```bash
bundle install
```

### 2. Executar os testes

```bash
cucumber
```
--- 

## 📊 Objetivo

Demonstrar a utilização de BDD na automação de testes, promovendo melhor comunicação entre negócio e tecnologia, além de garantir qualidade através de testes automatizados.

---

## 💡 Observações

Este projeto foi desenvolvido com foco em aprendizado e evolução na área de Qualidade de Software.
