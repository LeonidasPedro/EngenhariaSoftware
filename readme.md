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

## Exemplo:
```
@startuml Atividades
:Inserir cartão;
:Requisitar senha;
:Validar senha;
:Realizar saque;
@enduml
```

![](/PLantUML/Atividades.svg)

# Diagrama de sequência
## Diagrama de interação
- Representa uma sequência de mensagens trocadas entre objetos para realizar uma atividade.
- Cada mensagem é representada por uma linha de texto.
- Cada mensagem é representada por um símbolo de mensagem.
- Cada objeto é representado por um retângulo.
- Cada objeto é representado por um nome de classe.
- Cada objeto é representado por uma linha de vida.
- Cada objeto é representado por um símbolo de objeto.
- Cada objeto pode ser uma instância de uma classe.
- Cada objeto pode ser um ator.

## Exemplo:
```
@startuml Sequencia
actor Cliente
actor CaixaEletronico
Cliente -> CaixaEletronico : Fornecer senha
CaixaEletronico -> Cliente : Requisitar senha
CaixaEletronico -> Cliente : Validar senha
Cliente -> CaixaEletronico : Inserir cartão
Cliente -> CaixaEletronico : Realizar saque
@enduml
```

![](/PLantUML/Sequencia.svg)

# Diagrama de classes
## Diagrama de estrutura
- Representa a estrutura estática de um sistema.
- Cada classe é representada por um retângulo.
- Cada classe é representada por um nome de classe.
- Cada classe é representada por uma lista de atributos.
- Cada classe é representada por uma lista de operações.
- Cada classe pode ser uma classe abstrata.
- Cada classe pode ser uma classe concreta.
- Cada classe pode ser uma classe de interface.
- Cada classe pode ser uma classe de enumeração.
- Cada classe pode ser uma classe de anotação.
- Cada classe pode ser uma classe de exceção.
- Cada classe pode ser uma classe de teste.

## Exemplo:
```
@startuml Classes
class Cliente {
    -Nome: String
    -CPF: String
    -Endereço: String
    +getNome(): String
    +setNome(nome: String): void
    +getCPF(): String
    +setCPF(cpf: String): void
    +getEndereço(): String
    +setEndereço(endereço: String): void
}
class CaixaEletronico {
    -Senha: String
    -Saldo: Double
    +getSenha(): String
    +setSenha(senha: String): void
    +getSaldo(): Double
    +setSaldo(saldo: Double): void
}
@enduml
```

![](/PLantUML/Classes.svg)

# Diagrama de estados
## Diagrama de comportamento
- Representa o comportamento dinâmico de um sistema.
- Cada estado é representado por um círculo.
- Cada estado é representado por um nome de estado.
- Cada estado é representado por uma lista de ações.
- Cada estado é representado por uma lista de transições.
- Cada estado pode ser um estado inicial.
- Cada estado pode ser um estado final.
- Cada estado pode ser um estado interno.
- Cada estado pode ser um estado de submaquina.

## Exemplo:
```
@startuml Estados
[*] --> Inicial
Inicial --> Cliente
Cliente --> CaixaEletronico
CaixaEletronico --> Cliente
@enduml
```

![](/PLantUML/Estados.svg)

# Diagrama de componentes
## Diagrama de estrutura
- Representa a estrutura estática de um sistema.
- Cada componente é representado por um retângulo.
- Cada componente é representado por um nome de componente.
- Cada componente é representado por uma lista de interfaces.
- Cada componente é representado por uma lista de serviços.
- Cada componente é representado por uma lista de dependências.
- Cada componente é representado por uma lista de associações.
- Cada componente é representado por uma lista de agregações.
- Cada componente é representado por uma lista de composições.
- Cada componente é representado por uma lista de generalizações.
- Cada componente é representado por uma lista de especializações.
- Cada componente é representado por uma lista de realizações.
- Cada componente é representado por uma lista de pacotes.
- Cada componente é representado por uma lista de classes.
- Cada componente é representado por uma lista de interfaces.
- Cada componente é representado por uma lista de enums.
- Cada componente é representado por uma lista de anotações.
- Cada componente é representado por uma lista de exceções.
- Cada componente é representado por uma lista de testes.
- Cada componente pode ser um componente de software.
- Cada componente pode ser um componente de hardware.
- Cada componente pode ser um componente de interface.
- Cada componente pode ser um componente de banco de dados.
- Cada componente pode ser um componente de rede.
- Cada componente pode ser um componente de segurança.
- Cada componente pode ser um componente de controle.
- Cada componente pode ser um componente de teste.
- Cada componente pode ser um componente de usuário.
- Cada componente pode ser um componente de sistema.
- Cada componente pode ser um componente de serviço.
- Cada componente pode ser um componente de cliente.
- Cada componente pode ser um componente de servidor.
- Cada componente pode ser um componente de cliente/servidor.
- Cada componente pode ser um componente de distribuição.
- Cada componente pode ser um componente de sistema de informação.
- Cada componente pode ser um componente de sistema de software.

## Exemplo:
```
@startuml Componentes
component Cliente {
    -Nome: String
    -CPF: String
    -Endereço: String
    +getNome(): String
    +setNome(nome: String): void
    +getCPF(): String
    +setCPF(cpf: String): void
    +getEndereço(): String
    +setEndereço(endereço: String): void
}
component CaixaEletronico {
    -Senha: String
    -Saldo: Double
    +getSenha(): String
    +setSenha(senha: String): void
    +getSaldo(): Double
    +setSaldo(saldo: Double): void
}
@enduml
```

![](/PLantUML/Componentes.svg)

# Diagrama de implantação
## Diagrama de estrutura
- Representa a estrutura estática de um sistema.
- Cada artefato é representado por um retângulo.
- Cada artefato é representado por um nome de artefato.
- Cada artefato é representado por uma lista de dependências.
- Cada artefato é representado por uma lista de associa
- Cada artefato é representado por uma lista de agregações.

## Exemplo:
```
@startuml Implantação
artifact Cliente {
    -Nome: String
    -CPF: String
    -Endereço: String
    +getNome(): String
    +setNome(nome: String): void
    +getCPF(): String
    +setCPF(cpf: String): void
    +getEndereço(): String
    +setEndereço(endereço: String): void
}
artifact CaixaEletronico {
    -Senha: String
    -Saldo: Double
    +getSenha(): String
    +setSenha(senha: String): void
    +getSaldo(): Double
    +setSaldo(saldo: Double): void
}
@enduml
```

![](/PLantUML/Implantação.svg)

# Diagrama de pacotes
## Diagrama de estrutura
- Representa a estrutura estática de um sistema.
- Cada pacote é representado por um retângulo.
- Cada pacote é representado por um nome de pacote.
- Cada pacote é representado por uma lista de dependências.
- Cada pacote é representado por uma lista de associações.
- Cada pacote é representado por uma lista de agregações.
- Cada pacote é representado por uma lista de composições.
- Cada pacote é representado por uma lista de generalizações.
- Cada pacote é representado por uma lista de especializações.
- Cada pacote é representado por uma lista de realizações.
- Cada pacote é representado por uma lista de pacotes.
- Cada pacote é representado por uma lista de classes.
- Cada pacote é representado por uma lista de interfaces.
- Cada pacote é representado por uma lista de enums.
- Cada pacote é representado por uma lista de anotações.
- Cada pacote é representado por uma lista de exceções.
- Cada pacote é representado por uma lista de testes.

## Exemplo:
```
@startuml Pacotes
package Cliente {
    -Nome: String
    -CPF: String
    -Endereço: String
    +getNome(): String
    +setNome(nome: String): void
    +getCPF(): String
    +setCPF(cpf: String): void
    +getEndereço(): String
    +setEndereço(endereço: String): void
}