# 🚗 Sistema de Gerenciamento de Estacionamento

Este projeto foi desenvolvido como parte dos fundamentos da trilha .NET da **DIO**. O objetivo é gerenciar o fluxo de veículos em um estacionamento, controlando entradas, saídas e o cálculo automatizado de valores devidos.

## 🎯 O Desafio
O sistema permite ao operador interagir com um menu para:
1. **Cadastrar** um veículo pela placa.
2. **Remover** um veículo, calculando o valor total (Preço Inicial + Preço por Hora * Tempo Permanecido).
3. **Listar** todos os veículos ativos no pátio.

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

[Meu GitHub](https://github.com/larissaribeiro-dev)