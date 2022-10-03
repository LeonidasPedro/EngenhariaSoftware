# Plant UML é uma linguagem para ilustrar diagramas de projetos orientados a objetos.

## Exemplo:

```
@startuml Carro
class Carro

Motorista - Carro : dirige >
Carro *- Roda : Tem 4 >
Carro -- Pessoa : < owns

@enduml
```


![](/out/Carro.svg)


# Diagrama de casos de uso
## Requisitos de software
- Representação das funcionalidades externamente observaveis do sistema

- Dos elementos externos ao sistema que interagem com o mesmo.

## Equipe de clientes (validação)
- Aprovam o que o sistema deverá fazer
- Entendem o que o sistema deverá fazer

## Equipe de desenvolvedores
- Ponto de partida para refinar requisitos de software.

## Podem seguir um desenvolvimento dirigido a casos de uso.
-  Designer (projetista): encontrar classes
-  Testadores: usam como base para casos de teste

<br>

# Definindo modelo de caso

```



```

## Abstração do texto:
- Texto
 - Diagrama UML

## Atores:
- Cliente
- Caixa Eletrônico

## Funções:
- Fornecer senha
- Requisitar senha
- Validar senha
- Inserir cartão
- Realizar saque

## Ligamos os atores pelo sistema
```
@startuml Caso de uso
actor Cliente
actor CaixaEletronico

Cliente -> CaixaEletronico : Fornecer senha
CaixaEletronico -> Cliente : Requisitar senha
CaixaEletronico -> Cliente : Validar senha
Cliente -> CaixaEletronico : Inserir cartão
Cliente -> CaixaEletronico : Realizar saque
@enduml
```

![](/PLantUML/CasoDeUso.svg)

# Diagrama de atividades
## Diagrama de fluxo de atividades
- Representa uma sequência de atividades que ocorrem em um determinado contexto.
- O contexto é definido por um ator ou uma classe.
- Cada atividade é um bloco de ações que pode conter sub-atividades.
- Cada atividade pode ser executada por um ator ou uma classe.
- Cada atividade pode ser condicional.
- Cada atividade pode ser repetida.
- Cada atividade pode ser paralela.
- Cada atividade pode ser um ponto de extensão.
- Cada atividade pode ser um ponto de inclusão.

## Diagrama de atividades
- Representa uma sequência de atividades que ocorrem em um determinado contexto.
- O contexto é definido por um ator ou uma classe.
- Cada atividade é um bloco de ações que pode conter sub-atividades.
- Cada atividade pode ser executada por um ator ou uma classe.
- Cada atividade pode ser condicional.
- Cada atividade pode ser repetida.
- Cada atividade pode ser paralela.
- Cada atividade pode ser um ponto de extensão.
- Cada atividade pode ser um ponto de inclusão.

# Exercícios...