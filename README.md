# Global Solution - Computer Organization and Architecture

# Sistema IoT para Monitoramento de Cápsula Espacial

## Sobre o Projeto

Este projeto foi desenvolvido como parte da Global Solution da disciplina Computer Organization and Architecture.

O objetivo foi criar um sistema IoT capaz de monitorar condições internas de uma cápsula espacial simulada utilizando Arduino Uno. O sistema realiza a leitura de temperatura, luminosidade e vibração, exibindo as informações em tempo real em um display LCD e gerando alertas quando situações críticas são detectadas.

A proposta busca simular um ambiente semelhante ao encontrado em missões espaciais, onde o monitoramento constante das condições internas é fundamental para garantir a segurança da operação.

---

## Objetivo

Desenvolver um sistema embarcado capaz de monitorar variáveis importantes para o funcionamento seguro de uma cápsula espacial, utilizando sensores conectados ao Arduino e exibindo os dados em tempo real.

O sistema é capaz de:

- Monitorar temperatura;
- Monitorar luminosidade;
- Simular eventos de vibração;
- Exibir informações em um display LCD;
- Acionar alertas visuais;
- Detectar situações críticas individuais e combinadas.

---

## Componentes Utilizados

| Componente | Quantidade |
|------------|------------|
| Arduino Uno | 1 |
| Placa de Ensaio (Protoboard) | 1 |
| Display LCD 16x2 | 1 |
| Potenciômetro | 1 |
| Sensor de Temperatura (TMP36) | 1 |
| Fotoresistor (LDR) | 1 |
| Botão (Simulação de Vibração) | 1 |
| LEDs | 2 |
| Resistores | 4 |

---

## Funcionamento do Sistema

O sistema realiza o monitoramento contínuo das condições internas da cápsula espacial através dos sensores conectados ao Arduino.

### Temperatura

A temperatura é monitorada através do sensor TMP36.

Quando a temperatura ultrapassa o limite de 35°C, o sistema identifica uma condição de alerta e informa a situação no display LCD.

### Luminosidade

A luminosidade é monitorada através de um fotoresistor (LDR).

O Arduino realiza a leitura dos valores analógicos do sensor, que variam entre 0 e 1023. Durante os testes realizados no projeto, foi definido o valor 400 como limite mínimo de luminosidade. Quando a leitura fica abaixo desse valor, o sistema identifica uma condição de baixa iluminação e gera um alerta.

### Vibração

Como o simulador Tinkercad possui limitações para simular sensores de vibração, foi utilizado um botão para representar eventos de impacto ou turbulência na cápsula espacial.

Ao pressionar o botão, o sistema interpreta a ação como uma vibração e gera os alertas correspondentes.

### Sistema de Alertas

O sistema possui alertas individuais e combinados.

Alertas individuais:

- Temperatura Alta
- Luz Baixa
- Vibração

Alertas combinados:

- Temperatura Alta + Luz Baixa
- Temperatura Alta + Vibração
- Luz Baixa + Vibração

Quando uma condição crítica é identificada:

- O LED verde é desligado;
- O LED vermelho é acionado;
- Uma mensagem é exibida no display LCD.

---

## Circuito

```text
/images/circuito-completo.png
```
## Tecnologias Utilizadas

- Arduino Uno
- Linguagem C++
- Tinkercad

---

## Demonstração

Vídeo do projeto:

INSERIR LINK DO YOUTUBE

---

## Simulação no Tinkercad

https://www.tinkercad.com/things/33Dsxe93oew/editel?returnTo=%2Fdashboard&sharecode=Rd3HWKA_FkZgdwFympcHKZlpllKAeu8o8sVxIML7VQA

---

## Integrantes

- Leonardo Gabriel Sá Duarte - RM 569029
- Enzo Vieira de Nadai - RM 569985

---

## Aprendizados

Durante o desenvolvimento deste projeto foi possível aplicar conceitos relacionados a sistemas embarcados, sensores, programação em Arduino, monitoramento em tempo real e integração entre hardware e software.

Além do aprendizado técnico, o projeto permitiu compreender como sistemas de monitoramento podem auxiliar na identificação de situações críticas e na tomada de decisões em ambientes que exigem alta confiabilidade, como uma cápsula espacial.

---

## Conclusão

O sistema desenvolvido conseguiu monitorar as condições internas da cápsula espacial simulada, realizando a leitura dos sensores e acionando alertas automaticamente quando necessário.

Além do funcionamento do projeto, a atividade também contribuiu para o aprendizado prático sobre programação, sensores e integração entre hardware e software utilizando Arduino e Tinkercad.

Os resultados obtidos foram positivos e atenderam aos objetivos propostos pela atividade.
