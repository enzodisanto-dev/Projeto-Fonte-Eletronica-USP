# Projeto-Fonte-Eletrônica-USP

## Projeto foi desenvolvido para disciplina de eletrônica

## Instruções:

Desenvolver e montar uma fonte de alimentação retificadora com saída ajustável. O circuito deve ser projetado para converter a corrente alternada (CA) da rede elétrica em corrente contínua (CC) regulável.

A alimentação do sistema será feita por meio de uma tomada convencional, que fornece uma tensão eficaz de 127 V (equivalente a 179,6 V de pico) e frequência de 60 Hz. O objetivo final é que o circuito processe esse sinal e entregue na saída uma tensão contínua que possa ser controlada pelo usuário na faixa de 3 V a 12 V.

## Escolha dos Componentes

## Componentes

### 1. Entrada (Alimentação)
* **1x Fonte de Tensão AC:** 120Hz (Simulando a rede elétrica)
* **1x Transformador:** Diminui a tensão de entrada

### 2. Estágio de Retificação
* **4x Diodos Retificadores:** Converter a Corrente Alternada (AC) em Corrente Contínua (DC) pulsante.

### 3. Estágio de Filtragem
* **1x Capacitor:** 470µF Suaviza tensão pulsante

### 4. Estágio de Regulação de Tensão
* **1x Diodo Zener:** Estabelece a tensão de referência fixa do circuito.
* **1x Potenciômetro:** 10kΩ Permite calibrar a voltagem final circuito
* **1x Transistor (NPN):** Matém a voltagem estabilizada
* **1x Resistor:** 4.7kΩ
* **1x Resistor:** 3.3kΩ
* **1x Resistor:** 100Ω 

### 5. Estágio de Saída e Indicação (Carga)
* **1x LED (Vermelho):** Indicador de intensidade
* **1x Resistor:** 120Ω (Limitador de corrente).
* **1x Resistor:** 2.2kΩ (Limitador de corrente).

## O circuito

## Cáculo do capacitor

## Link do circuito - Falstad

- https://tinyurl.com/5336sruf


## Esquemático da PCB

## Vídeo Youtube

## Alunos:

#### Enzo Abreu di'Santo
#### Matheus de Oliveira Reis Pereira
#### Davi Miguel Moreira Resende
#### Daniel Meschiari da Silva

## Agradecimentos
