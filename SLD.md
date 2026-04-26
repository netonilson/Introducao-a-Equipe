# 3.1 O que é um seguidor de linha? 
### Um seguidor de linha é um robô autônomo capaz de, por meio de sensores e mapeamento, identificar o percurso e completá-lo no menor tempo possível, possuindo integração de componentes elétricos, mecânicos e sistema lógico 
# 3.2. Componentes principais 
## Quais são os principais componentes presentes em um seguidor de linha e quais são as suas funções? 
### Sensores ópticos = identificar o percurso e possíveis curvas.
### Controlador = processa as informações dos sentores e controla a velocidade dos motores.
### Sistemas de Movimentação = exemplo: motores com função fazer o robo se deslocaro para completar o percurso.

# Regulamento

## O que o robô precisa fazer para completar a pista?
### O robô deve partir da área de largada/chegada e percorrer todo o trajeto seguindo a linha branca no sentido correto, sem sair completamente da linha principal. Ao final do percurso, após ultrapassar a linha de chegada, ele deve permanecer totalmente dentro da área de largada/chegada e ficar parado por, no mínimo, 2 segundos.
## O que é considerado erro durante a prova?
### Os erros evidentes são o robô sair completamente do circuito, errar o caminho em um cruzamento e não parar ao fim do percurso. Erros fora do percurso em si também podem ocorrer, como o não seguimento das proporões obrigatõrias do robô, alteração de softwares, hardwares ou dimensões dentro da tomada.
## Existe limite de tamanho ou componentes?
### Sim, o Robô não pode exceder 250mm de comprimento, 250mm de largura e 200mm de altura, além de serem totalmente autônomos sem controladores externos. Fora isso cada competição pode ter especificidades proprias quanto às caracteristicas do robô.
## Como o robô é pontuado?
### Dentro da tomada, o Robô tem três chances de completar a pista, e a volta mais rápida é considerada.

# Escrita

## Qual é a lógica mais simples para permitir que o robô permaneça seguindo a linha?
### A utilização de dois sensores frontais, posicionados a uma distância ligeiramente maior que a espessura da linha, permite o controle de direção do robô. Quando nenhum dos sensores detecta a cor da linha, ambas as rodas giram na mesma velocidade (RPM), mantendo o movimento reto. Caso um dos sensores identifique a linha, a roda do mesmo lado tem sua velocidade reduzida ou é parada, corrigindo a trajetória e garantindo que o robô permaneça no percurso.
## Onde que ocorre o calculo de correção do robo para seguir a linha?
### O calculo ocorre no algoritmo de controle dentro do microcontrolador, com os dados adquiridos pelos sensores.
## A quantidade de sensores de linha é relevante?
### Sim, o número de sensores impacta diretamente na fluidez do movimento, uma vez que com maior informação sobre a posição do robô em relação á linha o movimento pode ser corrigido de forma mais correta e sem o movimento de "zigue zague" evidenciado pelo video, que deixa a volta mais lenta.
## O motor utilizado influencia em alguma coisa?
### Sim,  tipo de motor afeta diretamente a precisão, a velocidade e a estabilidade do robô ao seguir a linha
## Podemos utilizar qualquer tipo de roda, ou existe alguma lógica na escolha?
### Existe uma lógica, a roda deve ser escolhida visando estabilidade e velocidade do robô. As características importantes são a aderencia com o plano da corrida, proporções (diâmetro e expessura) e a prõpria massa da roda.
