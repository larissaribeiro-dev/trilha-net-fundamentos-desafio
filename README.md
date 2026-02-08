# DIO - Trilha .NET - Fundamentos
www.dio.me

## Desafio de projeto
Para este desafio, você precisará usar seus conhecimentos adquiridos no módulo de fundamentos, da trilha .NET da DIO.

## Contexto
Você foi contratado para construir um sistema para um estacionamento, que será usado para gerenciar os veículos estacionados e realizar suas operações, como por exemplo adicionar um veículo, remover um veículo (e exibir o valor cobrado durante o período) e listar os veículos.

## Proposta
Você precisará construir uma classe chamada "Estacionamento", conforme o diagrama abaixo:
![Diagrama de classe estacionamento](diagrama_classe_estacionamento.png)

A classe contém três variáveis, sendo:

**precoInicial**: Tipo decimal. É o preço cobrado para deixar seu veículo estacionado.

**precoPorHora**: Tipo decimal. É o preço por hora que o veículo permanecer estacionado.

**veiculos**: É uma lista de string, representando uma coleção de veículos estacionados. Contém apenas a placa do veículo.

A classe contém três métodos, sendo:

**AdicionarVeiculo**: Método responsável por receber uma placa digitada pelo usuário e guardar na variável **veiculos**.

**RemoverVeiculo**: Método responsável por verificar se um determinado veículo está estacionado, e caso positivo, irá pedir a quantidade de horas que ele permaneceu no estacionamento. Após isso, realiza o seguinte cálculo: **precoInicial** * **precoPorHora**, exibindo para o usuário.

**ListarVeiculos**: Lista todos os veículos presentes atualmente no estacionamento. Caso não haja nenhum, exibir a mensagem "Não há veículos estacionados".

Por último, deverá ser feito um menu interativo com as seguintes ações implementadas:
1. Cadastrar veículo
2. Remover veículo
3. Listar veículos
4. Encerrar

## 🧠 Conceitos .NET Aplicados
Neste projeto, apliquei fundamentos essenciais para qualquer desenvolvedor C#:
* **Manipulação de Coleções:** Uso de `List<string>` para gerenciar os dados em memória.
* **LINQ (Language Integrated Query):** Utilização do método `.Any()` para verificações rápidas e eficientes na lista.
* **Lógica de Programação:** Estruturas de repetição (`foreach`) e condicionais aninhadas.
* **Interação via Console:** Entrada e saída de dados via terminal, garantindo uma interface funcional para o usuário.

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** C#
* **Ambiente:** .NET 6.0 ou superior

## 📋 Regra de Cálculo
| Componente | Descrição |
|-------|-----------|
| **Preço Inicial** | Valor fixo cobrado apenas pela entrada do veículo. |
| **Preço por Hora** | Valor variável de acordo com o tempo de permanência. |
| **Fórmula** | `Valor Total = Preço Inicial + (Preço por Hora * Horas)` |

## 🚀 Como Executar
1. Clone o repositório.
2. Navegue até a pasta do projeto e execute `dotnet run`.
3. Siga as instruções do menu interativo no terminal.

---
A implementação conta com tratamento de sensibilidade de caixa (*Case Insensitive*) na busca de placas, aumentando a confiabilidade do sistema.