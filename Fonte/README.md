# Projeto 1: Fonte retificadora (12V ~ 3V)
Esse projeto consiste em uma fonte retificadora com uma tensão váriavel de 12V a 3V DC.

## Participantes
* Lourenço de Salles Roselino - 11796805
* Marco Antônio Ribeiro de Toledo - 11796419
* Milena Corrêa da Silva - 11795401

## Diagrama da Fonte
![falstad_print](https://i.imgur.com/pibB25M.png)
![eagle_print](https://cdn.discordapp.com/attachments/705588546890891336/726614224461103214/unknown.png)
![eagle_print2](https://cdn.discordapp.com/attachments/705588546890891336/726614089727737896/unknown.png)

#### [Link para o circuito no falstad](http://tinyurl.com/ybcu2mor)

### Componentes
|Nome   |Quantidade  |Especificações   |Explicações   | Preço |
|---|---|---|---|---|
|[Transformador](https://www.filipeflop.com/produto/transformador-trafo-12v-12v-500ma-bivolt/?gclid=Cj0KCQjwuJz3BRDTARIsAMg-HxW_dJmm9-pVBDe6o8W5fG-x5esHO2DdYG3BT5ngq7YSO-Iy3B0MDZ4aAn2MEALw_wcB) |1  | 127 – 220VAC (bivolt) 12V + 12V – 500mA  | Escolhemos este transformador por apresentar bom custo benefício em 12V + 12V e para ser utilizado transformando 127 VAC para 24 VAC, o que nos garante uma margem de erro confortável para quedas de tensão nos componentes|R$21,90 |
|[Diodo Retificador](https://www.filipeflop.com/produto/diodo-retificador-1n5408/)   |4  | 1N5408 | O diodo necessário precisava de um minimo de 25V de tensão de pico e 500mA (obtidos pela saída do transformador). No entanto, escolhemos um de 1000V e 3A por garantir uma margem de erro maior por baixo custo (esse definitivamente não vai queimar (･ω<)☆)| R$2,40 por 10 unidades |
|Capacitor  |2 | [[680uF 25V]](https://www.eletro-parts.com/produto_detalhes/p/TVRBMk16WT0=/132-+Eletrolitico+680uF+x+25V) [[470uF 25V]](https://www.baudaeletronica.com.br/capacitor-eletrolitico-470uf-25v.html) | Utilizamos um capacitor de 680uF pois juntamente com o outro ele estabiliza a corrente dentro dos 5% do padrão USB. Além disso, como a tensão total após o transformador é por volta de 24V ainda temos uma margem de segurança |R$10,00 por 20 unidades|
|[Diodo Zener](https://produto.mercadolivre.com.br/MLB-911630639-10-pcs-diodo-zener-13v-1w-1n4743frete-brasil-r1200-_JM?quantity=1#position=2&type=item&tracking_id=724e89c3-54f7-4462-9ed9-0cbeeed97948)   |1  | 13V - 1W | No geral, a corrente de pico (quando está em 3V) é aproximadamente 12 mA, o que resulta em uma voltagem de 156mW, mas o único diodo que conseguimos encontrar pra essa tensão (13V) foi este, então pelo menos temos, novamente, uma boa margem de erro|R$10,66 por 10 unidades|
|[Resistência]()   | 1  | 1.2kohm  | Utilizada para limitar a tensão no zener e para que está fique na faixa de 13V  | |
|[Resistência](https://www.magazineluiza.com.br/20-resistor-22-ohms-1-4w-casa-da-robotica/p/ccdb3ajfbe/rc/rcnm/?&1=1&seller_id=casadarobotica&&utm_source=google&utm_medium=pla&utm_campaign=&partner_id=54222&gclid=CjwKCAjw_-D3BRBIEiwAjVMy7MiFkfwRfk52JnGeVzgOdv1REiqpxv2xg8C84aXCgl5YQpDI3HxaqRoCC-MQAvD_BwE)    | 1   | 22ohm| Uma resistência foi utilizada para controlar a corrente que passa pelo NPN e não estora-lo e a outra representa o load|R$ 2.99 por 20 unidades|
|[Potenciômetro](https://www.submarino.com.br/produto/1486223377/potenciometro-linear-tipo-b-5k?WT.srch=1&acc=d47a04c6f99456bc289220d5d0ff208d&epar=bp_pl_00_go_g35164&gclid=Cj0KCQjw3Nv3BRC8ARIsAPh8hgJ1zi-D6z9f-GZEor7-OQ692x4VBREkFTeZVXomAuMNY7Gf06GorZ0aAunVEALw_wcB&i=5e350c4649f937f625c487c0&o=5e34ac65f8e95eac3d165fa6&opn=XMLGOOGLE&sellerid=16569609000116)   |1   | 5kohm  | Na teoria, só precisariamos de um potenciometro de 3.3kohm com uma resistencia de 2.2ohm, mas como não encontramos tal para vender mudamos para um potenciometro  | R$ 6,61  |

#### Link para o vídeo explicativo
... (em construção)
