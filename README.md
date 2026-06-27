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

## Cáculos do circuito
### Dados
- razão do transformador: 6.7
- capacitância: 470 μF
- tensão do zener: 13 V
- resistor em série com zener: 4.7 Ω
- resistência do potenciômetro: 10 Ω
- resistor do celular: 120 Ω
- ganho do transistor: 100

### Calculando
- TRANSFORMAÇÃO
	- tensão de pico: 127 V x $\sqrt{2}$ = 180 V
	- tensão secundário: $\frac{180}{6.7}$ = 26,86 V ~ 27 V
- RETIFICAÇÃO
	- tensão máxima: 27 V - 1.4 V = 25.6 V
- CORRENTES
	- corrente de carga: $\frac{12}{120}$ = 100 mA
	- corrente da base do transistor: $\frac{0.1}{100}$ = 0.1 mA
	- corrente zener: $\frac{25.6 - 13}{4700}$ = 2,6 mA
	- corrente LED: $\frac{25.6 - 1.7}{2200}$ = 1 mA
	- corrente total: 2.6 + 1 = 3.6 mA
- RIPPLE
	- tensão ripple: $\frac{3.6}{120}$ = 0,03 V
	- tensão retificada mínima: 25.6 - 0.03 = 25.57 V
- REGULAÇÃO
	- tensão na base: ${13}\times{\frac{R}{10000}}$
	- tensão na saída: ${13}\times{\frac{R}{10000}} - {0.7}$
	- com potenciômetro no mínimo:
		- tensão na base: 0 V
		- tensão na saída: -0.7 V ~ 0 V
	- com potenciômetro no máximo:
		- tensão na base: 13 V
		- tensão na saída: 12.3 V


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
