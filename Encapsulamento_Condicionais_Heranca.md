# 📘 Exercício de Fixação – Encapsulamento, Condicionais e Herança

## Disciplina: Programação Orientada a Objetos com JavaScript

### Conteúdos Trabalhados

* Classes e Objetos
* Visibilidade de atributos
* Encapsulamento
* Getters e Setters
* Estruturas Condicionais
* Herança
* Reutilização de Código
* Instanciação de Objetos

---

# 🎯 Objetivos de Aprendizagem

Ao concluir esta atividade o estudante deverá ser capaz de:

* Criar classes utilizando JavaScript moderno;
* Declarar atributos privados utilizando `#`;
* Implementar métodos Getters e Setters;
* Aplicar validações utilizando estruturas condicionais;
* Utilizar herança através da palavra-chave `extends`;
* Reutilizar métodos herdados;
* Instanciar objetos e testar seus comportamentos;
* Compreender a importância do encapsulamento na proteção dos dados.

---

# 📖 Contextualização

Uma instituição de ensino está desenvolvendo um sistema para cadastro de pessoas.

Na primeira versão do sistema foi criada uma classe chamada `Pessoa`, responsável por armazenar informações básicas como nome e e-mail.

Agora será necessário expandir esse sistema para permitir o cadastro de alunos e professores, aproveitando os conceitos de herança e encapsulamento estudados em sala.

Seu papel será implementar as classes necessárias e realizar os testes para verificar seu funcionamento.

---

# 🧩 Parte 1 – Classe Pessoa

Crie um arquivo chamado:

```javascript
Pessoa.js
```

## Requisitos

A classe deve possuir os seguintes atributos privados:

```javascript
#nome
#email
```

## Métodos Obrigatórios

```javascript
setNome()
getNome()

setEmail()
getEmail()
```

## Regras de Negócio

### Método setNome()

* receber um parâmetro chamado `nome`;
* verificar se o valor não está vazio;
* armazenar o valor apenas quando válido;
* retornar `true` quando a operação for realizada;
* retornar `false` quando o valor estiver vazio.

### Método setEmail()

* receber um parâmetro chamado `email`;
* verificar se o valor não está vazio;
* armazenar o valor apenas quando válido;
* retornar `true` quando a operação for realizada;
* retornar `false` quando o valor estiver vazio.

---

# 🧩 Parte 2 – Classe Aluno

Crie um arquivo chamado:

```javascript
Aluno.js
```

A classe deverá herdar da classe `Pessoa` utilizando:

```javascript
extends
```

## Novo Atributo

```javascript
#matricula
```

## Métodos

```javascript
setMatricula()
getMatricula()
```

## Regra

A matrícula somente poderá ser cadastrada quando possuir algum valor.

---

# 🧩 Parte 3 – Classe Professor

Crie um arquivo chamado:

```javascript
Professor.js
```

A classe deverá herdar da classe `Pessoa`.

## Atributo

```javascript
#disciplina
```

## Métodos

```javascript
setDisciplina()
getDisciplina()
```

A disciplina não poderá ser vazia.

---

# 🧪 Parte 4 – Arquivo de Testes

Criar um arquivo chamado:

```javascript
usaPessoas.js
```

## Teste 1 – Pessoa Válida

Criar um objeto:

```javascript
const p = new Pessoa();
```

Cadastrar:

```text
Nome: João Silva
Email: joao@email.com
```

Exibir os dados utilizando os métodos Getters.

---

## Teste 2 – Pessoa Inválida

Criar um objeto:

```javascript
const p2 = new Pessoa();
```

Cadastrar:

```text
Nome: ""
Email: ""
```

Exibir mensagens adequadas quando ocorrer erro.

---

## Teste 3 – Aluno Válido

Criar um objeto:

```javascript
const a = new Aluno();
```

Cadastrar:

```text
Nome: Maria
Email: maria@email.com
Matrícula: 2025001
```

Exibir:

```text
Nome:
Email:
Matrícula:
```

---

## Teste 4 – Aluno Inválido

Cadastrar:

```text
Nome: Pedro
Email: ""
Matrícula: ""
```

Verificar quais métodos retornam `false`.

---

## Teste 5 – Professor Válido

Criar um objeto:

```javascript
const prof = new Professor();
```

Cadastrar:

```text
Nome: Carlos
Email: carlos@email.com
Disciplina: Programação Web
```

---

## Teste 6 – Professor Inválido

Cadastrar:

```text
Nome: Ana
Email: ana@email.com
Disciplina: ""
```

Exibir mensagem informando erro no cadastro da disciplina.

---

# ⭐ Desafio Extra 1 – Validação de E-mail

Modificar o método:

```javascript
setEmail()
```

para aceitar apenas e-mails contendo:

```text
@
```

Exemplo:

```javascript
if(email.includes("@"))
```

---

# ⭐ Desafio Extra 2 – Validação de Matrícula

Modificar:

```javascript
setMatricula()
```

para aceitar somente matrículas com pelo menos 6 caracteres.

---

# ⭐⭐ Desafio Avançado

Criar uma nova classe:

```javascript
Coordenador
```

que herde de:

```javascript
Professor
```

Adicionar:

```javascript
#setor
```

Implementar:

```javascript
setSetor()
getSetor()
```

Estrutura esperada:

```text
Pessoa
   ↑
Professor
   ↑
Coordenador
```

---

# 📌 Questões Teóricas

1. O que é encapsulamento?
2. Qual a vantagem de utilizar atributos privados?
3. Qual a diferença entre getter e setter?
4. O que faz a palavra-chave `extends`?
5. Uma classe filha pode utilizar métodos da classe pai?
6. Por que utilizar validações dentro dos métodos?
7. Qual a diferença entre herança e reutilização por cópia?

---

# 📌 Critérios de Avaliação

| Critério               | Pontos |
| ---------------------- | ------ |
| Classe Pessoa          | 1,5    |
| Encapsulamento correto | 1,5    |
| Uso de condicionais    | 1,5    |
| Classe Aluno           | 1,5    |
| Classe Professor       | 1,5    |
| Arquivo de testes      | 1,5    |
| Questões teóricas      | 1,0    |

**Total: 10,0 pontos**

---

# 🚀 Desafio Final

Implemente um menu simples utilizando:

```javascript
prompt()
```

ou

```javascript
readline()
```

que permita:

```text
1 - Cadastrar Pessoa
2 - Cadastrar Aluno
3 - Cadastrar Professor
4 - Listar Dados
5 - Sair
```

Este desafio servirá como preparação para os próximos conteúdos de:

* Composição de Objetos;
* Coleções de Objetos;
* Persistência de Dados.
