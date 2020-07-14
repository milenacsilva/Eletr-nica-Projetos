# Projeto 1: Fonte retificadora (12V ~ 3V)
Esse projeto consiste em uma fonte retificadora com uma tensão váriavel de 12V a 3V DC.

## Participantes
<a href="https://github.com/roselino-quatro"><img src="https://avatars3.githubusercontent.com/u/43501582?s=460&u=607eaa89f7d1d4117ad8e3b2059d7fd24e1c0b45&v=4" title="rafa-quatro" width="80" height="80"></a>
<a href="https://github.com/Ocramoi"><img src="https://avatars1.githubusercontent.com/u/9422402?s=460&v=4" title="ocramoi" width="80" height="80"></a>
<a href="https://github.com/milenacsilva"><img src="https://avatars2.githubusercontent.com/u/61664263?s=460&v=4" title="milenacsilva" width="80" height="80"></a>

Lourenço de Salles Roselino - **11796805**\
Marco Antônio Ribeiro de Toledo - **11796419**\
Milena Corrêa da Silva - **11795401**

## Diagrama da Fonte (FALSTAD)
![falstad_print](https://i.imgur.com/WWNlFE1.gif)
Obs.: o novo circuito, que pode ser acessado pelo link, tem um diodo zener a mais no segundo capacitor para evitar o refluxo
### [Link para o circuito](http://tinyurl.com/ycd7924y)
### [Link para o vídeo explicativo](https://youtu.be/yuhNi4NMBbg)

## Projeto Esquemático e PCB (EAGLE)
![eagle_print](https://cdn.discordapp.com/attachments/705588546890891336/726614224461103214/unknown.png) 
![eagle_print2](https://cdn.discordapp.com/attachments/705588546890891336/726614089727737896/unknown.png)


### Componentes
|Nome|Quantidade|Especificações|Explicações|Preço Unitário|
|---|---|---|---|---|
| **Interruptor** |**1**| **250Vac-3A**| Apenas para ligar e desligar o circuito | [R$3,49](https://www.americanas.com.br/produto/212542071/mts-101-chave-alavanca-2-terminais-desliga-liga?WT.srch=1&acc=e789ea56094489dffd798f86ff51c7a9&epar=bp_pl_00_go_pla_aic_geral_gmv&gclid=CjwKCAjw_-D3BRBIEiwAjVMy7A9KBPJMsUWKBYhhVwBYxDCUsOgVK7NK1RYUPgc3qsUI06BmjM9sBBoCqrAQAvD_BwE&i=5d712b2d49f937f6250d8225&o=5d7bf2046c28a3cb50a3896b&opn=YSMESP&sellerid=10428528000110#info-section) | 
|**Transformador**|**1**| **127 – 220VAC (bivolt) 12V + 12V – 500mA**  | Escolhemos este transformador por apresentar bom custo benefício em 12V + 12V e para ser utilizado transformando 127 VAC para 24 VAC, o que nos garante uma margem de erro confortável para quedas de tensão nos componentes|[R$21,90](https://www.filipeflop.com/produto/transformador-trafo-12v-12v-500ma-bivolt/?gclid=Cj0KCQjwuJz3BRDTARIsAMg-HxW_dJmm9-pVBDe6o8W5fG-x5esHO2DdYG3BT5ngq7YSO-Iy3B0MDZ4aAn2MEALw_wcB) |
|**Diodo Retificador**|**4**| **1N5408** | O diodo necessário precisava de um minimo de 25V de tensão de pico e 500mA (obtidos pela saída do transformador). No entanto, escolhemos um de 1000V e 3A por garantir uma margem de erro maior por baixo custo (esse definitivamente não vai queimar (･ω<)☆)| [R$0,24](https://www.filipeflop.com/produto/diodo-retificador-1n5408/)|
|**Capacitor**|**2**| **680uF-25V e 470uF-25V** | Utilizamos um capacitor de 680uF pois juntamente com o outro ele estabiliza a corrente dentro dos 5% do padrão USB. Além disso, como a tensão total após o transformador é por volta de 24V ainda temos uma margem de segurança |[R$0,60](https://www.eletro-parts.com/produto_detalhes/p/TVRBMk16WT0=/132-+Eletrolitico+680uF+x+25V) [R$0,33](https://www.baudaeletronica.com.br/capacitor-eletrolitico-470uf-25v.html)|
|**Diodo Zener**|**1**| **13V - 1W** | No geral, a corrente de pico (quando está em 3V) é aproximadamente 12 mA, o que resulta em uma voltagem de 156mW, mas o único diodo que conseguimos encontrar pra essa tensão (13V) foi este, então pelo menos temos, novamente, uma boa margem de erro|[R$1,05](https://produto.mercadolivre.com.br/MLB-911630639-10-pcs-diodo-zener-13v-1w-1n4743frete-brasil-r1200-_JM?quantity=1#position=2&type=item&tracking_id=724e89c3-54f7-4462-9ed9-0cbeeed97948)|
|**Resistência**|**1**| **1k2ohm - 1/4W** | Utilizada para limitar a tensão no zener de modo que está fique na faixa de 13V  |[R$1,24](https://produto.mercadolivre.com.br/MLB-1430649347-resistor-1k2-x-14w-5-tolerancia-envio-por-carta-_JM?matt_tool=79246729&matt_word=&gclid=CjwKCAjw_-D3BRBIEiwAjVMy7BmHKkFoWHFlQpg0uiS6qf9cVWsYGtSsGgh42hpRstRQxxA4gbsizBoCq0IQAvD_BwE) |
|**Resistência**|**1**| **22ohm**| Essa resistência foi utilizada para controlar a corrente que passa pelo NPN e não estora-lo |[R$0,145](https://www.casadarobotica.com/componentes-eletronicos/componentes/resistor/20-resistor-22-ohms-14w)|
|**Potenciômetro**|**1**| **3k3ohm**  | Parte do sistema controlador, junto com a resistência de 2k2ohm garante uma tensão máxima de aproximadamente 12V e mínima de 3V na saída | [R$9,40](https://www.baudaeletronica.com.br/potenciometro-linear-de-3k3-l40-23mm.html)|
|**Resistência**|**1**| **2k2ohm** | Novamente, faz parte do controlador | [R$0,10](https://www.usinainfo.com.br/resistores/resistor-2k2-14w-kit-com-10-unidades-3772.html) |
|**Resistência**|**1**| **27ohm** | Representa o load | [R$0,05](https://produto.mercadolivre.com.br/MLB-1559727072-resistor-27r-ou-27-ohms-cr25-14w-5-pacote-c-1000-pecas-_JM?matt_tool=79246729&matt_word&gclid=CjwKCAjw_-D3BRBIEiwAjVMy7GPkKLxWNdczv_iB6-YxnClYdcXWfBU5fFMdJMur2VC7c6ZDHZ9zEBoCkBgQAvD_BwE&quantity=1) |

