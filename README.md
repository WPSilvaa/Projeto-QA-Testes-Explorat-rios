# Projeto QA – Testes Exploratórios

# 📌 Objetivo

Este projeto foi criado com o objetivo de demonstrar conhecimentos práticos em testes exploratórios aplicados em aplicações web.

Os cenários foram elaborados simulando situações reais encontradas no dia a dia da área de Quality Assurance (QA), com foco na identificação de falhas funcionais, inconsistências de comportamento, problemas de usabilidade e validação de regras de negócio.

---

# 🧠 O que são Testes Exploratórios?

Testes exploratórios são uma abordagem onde o profissional realiza testes simultaneamente ao aprendizado da aplicação.

Diferente de testes totalmente roteirizados, os testes exploratórios incentivam:

* pensamento crítico
* criatividade
* investigação
* identificação de comportamentos inesperados
* análise da experiência do usuário

---

# 🎯 Objetivos dos Testes

* Validar comportamento da aplicação
* Identificar falhas funcionais
* Encontrar inconsistências de interface
* Avaliar usabilidade
* Verificar regras de negócio
* Simular comportamento real do usuário

---

# 🧪 Cenário Testado

## Aplicação simulada

Sistema web de gerenciamento de produtos.

Funcionalidades analisadas:

* Login
* Cadastro de produtos
* Pesquisa de produtos
* Exclusão de registros
* Carrinho de compras
* Logout

---

# 🔎 Testes Exploratórios – Login

## Cenário 1 – Tentativas inválidas consecutivas

### Objetivo

Validar comportamento do sistema após múltiplas tentativas incorretas.

### Exploração realizada

* Inserção de senha inválida repetidamente
* Alteração de letras maiúsculas/minúsculas
* Uso de caracteres especiais

### Resultado esperado

Sistema bloquear acesso temporariamente após limite de tentativas.

### Possível risco encontrado

Sistema sem limitação de tentativas pode permitir ataques de força bruta.

---

## Cenário 2 – Campos vazios

### Exploração realizada

* Clique em “Entrar” sem preencher campos
* Preenchimento parcial
* Espaços em branco

### Resultado esperado

Sistema deve validar obrigatoriedade dos campos.

### Observações

Mensagens de erro devem ser claras para o usuário.

---

# 📦 Testes Exploratórios – Cadastro de Produtos

## Cenário 3 – Inserção de valores inválidos

### Exploração realizada

* Preço negativo
* Letras no campo valor
* Quantidade negativa
* Caracteres especiais

### Resultado esperado

Sistema deve impedir cadastro inválido.

### Possíveis falhas encontradas

* Falta de validação
* Aceite de valores incorretos
* Quebra de layout

---

## Cenário 4 – Limite de caracteres

### Exploração realizada

* Inserção de textos extremamente longos
* Copiar e colar conteúdo acima do limite esperado

### Resultado esperado

Sistema deve limitar quantidade de caracteres.

### Riscos

* Quebra visual
* Erro de banco de dados
* Lentidão

---

# 🛒 Testes Exploratórios – Carrinho de Compras

## Cenário 5 – Atualização rápida de quantidade

### Exploração realizada

* Cliques rápidos nos botões de quantidade
* Alterações consecutivas
* Remoção simultânea de produtos

### Resultado esperado

Sistema deve atualizar valores corretamente.

### Possíveis problemas

* Valores inconsistentes
* Duplicidade de itens
* Total incorreto

---

## Cenário 6 – Cupom inválido

### Exploração realizada

* Inserção de códigos aleatórios
* Caracteres especiais
* Cupons expirados

### Resultado esperado

Sistema deve rejeitar cupons inválidos.

---

# 🐞 Bugs Simulados Encontrados

## BUG-001 – Sistema aceita preço negativo

### Severidade

Alta

### Impacto

Produtos podem ser cadastrados com valores inválidos.

### Evidência

Cadastro realizado com valor “-100”.

---

## BUG-002 – Sistema permite login ilimitado

### Severidade

Crítica

### Impacto

Possível vulnerabilidade de segurança.

---

## BUG-003 – Campo nome quebra layout

### Severidade

Média

### Impacto

Problema visual e possível inconsistência de dados.

---

# 📋 Técnicas Exploratórias Utilizadas

* Teste baseado em experiência do usuário
* Testes negativos
* Validação de limites
* Testes de comportamento inesperado
* Exploração de fluxo alternativo
* Validação de mensagens do sistema

---

# 📚 Conceitos Trabalhados

* QA Manual
* Testes Exploratórios
* Testes Funcionais
* Regras de Negócio
* Usabilidade
* Registro de Bugs
* Análise de Risco

---

# 🚀 Próximos Passos

* Automatizar cenários críticos
* Criar evidências visuais
* Integrar testes com Selenium
* Criar testes de API
* Estruturar suíte de regressão

---

# 👨‍💻 Autor

Willian Pereira

Projeto desenvolvido para fins de estudo e fortalecimento de portfólio profissional na área de Quality Assurance (QA).

