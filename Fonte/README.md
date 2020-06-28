# Projeto 1: Fonte retificadora (12V ~ 3V)
Esse projeto consiste em uma fonte retificadora com uma tensão váriavel de 12V a 3V DC.

## Participantes
* Lourenço de Salles Roselino - 11796805
* Marco Antônio Ribeiro de Toledo - 11796419
* Milena Corrêa da Silva - 11795401

## Diagrama da Fonte
![falstad_print](https://i.imgur.com/IxdalQt.png)
![eagle_print](https://cdn.discordapp.com/attachments/705588546890891336/726603726617575434/unknown.png)

#### [Link para o circuito no falstad](http://tinyurl.com/y8eeqs6w)

### Componentes
|Nome   |Quantidade  |Especificações   |Explicações   | Preço |
|---|---|---|---|---|
|[Transformador](https://www.filipeflop.com/produto/transformador-trafo-12v-12v-500ma-bivolt/?gclid=Cj0KCQjwuJz3BRDTARIsAMg-HxW_dJmm9-pVBDe6o8W5fG-x5esHO2DdYG3BT5ngq7YSO-Iy3B0MDZ4aAn2MEALw_wcB) |1  | 127 – 220VAC (bivolt) 12V + 12V – 500mA  | Escolhemos este transformador por apresentar bom custo benefício em 12V + 12V e para ser utilizado transformando 127 VAC para 24 VAC, o que nos garante uma margem de erro confortável para quedas de tensão nos componentes|R$21,90 |
|[Diodo Retificador](https://www.filipeflop.com/produto/diodo-retificador-1n5408/)   |4  | 1N5408 | O diodo necessário precisava de um minimo de 25V de tensão de pico e 500mA (obtidos pela saída do transformador). No entanto, escolhemos um de 1000V e 3A por garantir uma margem de erro maior por baixo custo (esse definitivamente não vai queimar (･ω<)☆)| R$2,40 por 10 unidades |
|Capacitor  |2 | [[680uF 25V]](https://www.eletro-parts.com/produto_detalhes/p/TVRBMk16WT0=/132-+Eletrolitico+680uF+x+25V) [[470uF 25V]](https://www.baudaeletronica.com.br/capacitor-eletrolitico-470uf-25v.html) | Utilizamos um capacitor de 680uF pois juntamente com o outro ele estabiliza a corrente dentro dos 5% do padrão USB. Além disso, como a tensão total após o transformador é por volta de 24V ainda temos uma margem de segurança |R$10,00 por 20 unidades|
|[Diodo Zener](https://produto.mercadolivre.com.br/MLB-911630639-10-pcs-diodo-zener-13v-1w-1n4743frete-brasil-r1200-_JM?quantity=1#position=2&type=item&tracking_id=724e89c3-54f7-4462-9ed9-0cbeeed97948)   |1  | 13V - 1W | No geral, a corrente de pico (quando está em 3V) é aproximadamente 12 mA, o que resulta em uma voltagem de 156mW, mas o único diodo que conseguimos encontrar pra essa tensão (13V) foi este, então pelo menos temos, novamente, uma boa margem de erro|R$10,66 por 10 unidades|
|[Resistência](https://produto.mercadolivre.com.br/MLB-1360686564-100un-resistor-3w-680-ohms-680r-_JM?matt_tool=79246729&matt_word&gclid=Cj0KCQjw3Nv3BRC8ARIsAPh8hgIZthx3jkiPw2VOVmCo1oc2xP3LB-l-BSqcjDnmkyEKC1g_jZUm-xMaAg-5EALw_wcB&quantity=1)   | 1  | 680ohm  | Utilizada para limitar a tensão no zener e para que está fique na faixa de 13V  | R$ 33,99 pro 100 unidades  |
|Resistência    | 2   | 22ohm| Uma resistência foi utilizada para controlar a corrente que passa pelo NPN e não estora-lo e a outra representa o load|
|Resistência  | 1   | 3.1kohm    |    |
|Potenciômetro   |1   |   |   |   |

#### Link para o vídeo explicativo
... (em construção)
