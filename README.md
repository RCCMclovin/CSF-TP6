# CSF-TP6

Este trabalho usa o mesmo código das aulas anteriores.

## Medição de Link Budget

O objetivo deste trabalho é calcular o link budget para uma comunicação sem fio entre dois dispositivos, uma métrica que avalia a relação entre a potência transmitida e a potência recebida em um sistema de comunicação.

![Link Budget](./img/Link%20Budget.png)

### Procedimento

+ Um dispositivo deverá atuar como transmissor, transmitindo o sinal com uma potência conhecida (PT), enquanto outro, a uma distância conhecida, atuará como receptor.

+ Medir a potência recebida (PR)

+ Usar a seguinte fórmula: **Link Budget = PT − PR + GT − Lpath + GR**

  + PT: Potência transmitida (conhecida).
  + PR: Potência recebida (medida).
  + GT: Ganho da antena transmissora.
  + Lpath: Perda de propagação do sinal (dependente da distância e ambiente).
  + GR: Ganho da antena receptora.

+ Calcular a Link Margin (também conhecida como Fade Margin), levando em consideração a sensibilidade do receptor descrita na documentação do WiFi LoRa 32.

![RX Sensibility](./img/heltec%20sensitivity.png)

+ Repetir as medições com, ao menos, uma outra antena no transmissor, para haver comparações.

### Relatório

+ Comparar os resultados observados com os resultados teóricos obtidos através das fórmulas estudadas nas aulas teóricas.

+ Discutir as principais fontes de perda (atenuação, interferência, obstáculos) e como otimizar o link budget.

+ Pesquisar qual a Link Margin típica em um sistema IoT e comparar os resultados obtidos com isso.

+ Discutir a importância de otimizar o link budget para garantir uma conexão confiável.

+ Comparar os resultados com uma ou mais outra antena.
