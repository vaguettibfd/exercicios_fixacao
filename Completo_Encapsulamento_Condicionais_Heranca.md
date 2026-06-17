# Exercício de Fixação – Encapsulamento, Condicionais e Herança

## Disciplina: Programação Orientada a Objetos com JavaScript

### Conteúdos Trabalhados
- Classes e Objetos
- Visibilidade de atributos
- Encapsulamento
- Getters e Setters
- Estruturas Condicionais
- Herança
- Reutilização de Código
- Instanciação de Objetos

## Objetivos de Aprendizagem
- Criar classes utilizando JavaScript moderno;
- Declarar atributos privados utilizando #;
- Implementar métodos Getters e Setters;
- Aplicar validações utilizando estruturas condicionais;
- Utilizar herança através da palavra-chave extends;
- Reutilizar métodos herdados.

## Parte 1 – Classe Pessoa
Crie a classe Pessoa com os atributos privados:
- #nome
- #email

Implemente:
- setNome()
- getNome()
- setEmail()
- getEmail()

As validações devem retornar true para valores válidos e false para valores vazios.

## Parte 2 – Classe Aluno
Crie a classe Aluno herdando de Pessoa.

Adicionar:
- #matricula

Implementar:
- setMatricula()
- getMatricula()

## Parte 3 – Classe Professor
Crie a classe Professor herdando de Pessoa.

Adicionar:
- #disciplina

Implementar:
- setDisciplina()
- getDisciplina()

## Parte 4 – Arquivo de Testes
Crie o arquivo usaPessoas.js e realize os testes de Pessoa, Aluno e Professor com dados válidos e inválidos.

## Desafio Extra
Modificar setEmail() para aceitar apenas emails contendo @.

## Desafio Avançado
Criar a classe Coordenador herdando de Professor e adicionar o atributo #setor.

## Questões Teóricas
1. O que é encapsulamento?
2. Qual a vantagem de utilizar atributos privados?
3. Qual a diferença entre getter e setter?
4. O que faz a palavra-chave extends?
5. Uma classe filha pode utilizar métodos da classe pai?

## Critérios de Avaliação
- Classe Pessoa
- Encapsulamento
- Condicionais
- Classe Aluno
- Classe Professor
- Arquivo de testes
- Questões teóricas
