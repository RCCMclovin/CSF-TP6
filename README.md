# CSF-TP6

Este trabalho usa o mesmo código das aulas anteriores.

## Objetivos

+ Compreender e calcular o link budget em um sistema de comunicação sem fio, analisando a influência dos ganhos e perdas do sistema.

+ Avaliar o impacto de diferentes antenas, frequências, obstáculos e distâncias.

+ Verificar se o sistema opera em campo distante (região de Fraunhofer).

+ Comparar resultados teóricos com medições práticas.

+ Desenvolver habilidades em experimentação, registro, análise crítica e cooperação.

Para calcular o link budget para uma comunicação sem fio entre dois dispositivos, considere a figura abaixo.

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

+ Determine se a condição de campo distante (Fraunhofer) é satisfeita.

+ Se possível, realize a atividade em ambientes distintos (ex: Lab Maker vs. área externa) para reforçar o impacto do ambiente na propagação do sinal.

### Discussão

+ Identificar os elementos básicos de um sistema de comunicação sem fio;

+ Discutir os desafios para programar a transmissão e recepção dos dados;

+ Medir a força do sinal recebido durante a transmissão;

+ Calcular o ganho das antenas;

+ Quais fatores do ambiente influenciaram mais o link budget observado?

+ A comunicação em algum momento deixou de atender à margem de desvanecimento recomendada (10–25 dB)?

+ A equação de Friis se aproximou dos valores medidos? Onde houve maior discrepância?

+ Discutir as principais fontes de perda (atenuação, interferência, obstáculos) e como otimizar o link budget.

+ Como otimizar esse sistema para maior alcance com menor potência?

### Relatório

Elaborar um relatório descrevendo os procedimentos, os resultados e conclusões.
O relatório deverá conter:

+ Identificação do grupo e datas das medições.

+ Descrição dos equipamentos e código usado.

+ Tabela com resultados medidos e calculados: PT, RSSI, FSPL, fade margin.

+ Gráficos (recomendado) comparando distância × potência recebida.

+ Fotos ou esquemas dos ambientes de teste.

+ Discussão técnica (ver itens acima).

+ Conclusões com sugestões de melhoria no sistema.
