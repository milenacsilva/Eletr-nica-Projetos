# Projeto 1: Fonte retificadora (12V ~ 3V)
Esse projeto consiste em uma fonte retificadora com uma tensão váriavel de 12V a 3V DC.

## Participantes
* Lourenço de Salles Roselino - 11796805
* Marco Antônio Ribeiro de Toledo - 11796419
* Milena Corrêa da Silva - 11795401

## Diagrama da Fonte
[falstad](http://tinyurl.com/y8eeqs6w)

### Componentes
|Nome   |Quantidade  |Especificações   |Explicaçoẽs   | Preço |
|---|---|---|---|---|
|Transformador   |1  | 127 – 220VAC (bivolt) 12V + 12V – 500mA  | Escolhemos este transformador por apresentar bom custo benefício em 12V + 12V e para ser utilizado transformando 127 VAC para 24 VAC, o que nos garante uma margem de erro confortável para quedas de tensão nos componentes|R$21,90 |
|Diodo Retificador   |4  | 1N5408 | O diodo necessário precisava de um minimo de 25V de tensão de pico e 500mA (obtidos pela saída do transformador). No entanto, escolhemos um de 1000V e 3A por garantir uma margem de erro maior por baixo custo (este definitivamente não vai queimar (･ω<)☆)| R$2,40 por 10 unidades |
|Capacitor   |1 | 2.2mf 100v  |Utilizando a fórmula C = (amperagem [mili amperes] * tempo [mili segundos])/voltagem [volts], calculamos que a  capacitancia necessária será 2.075 mF com 25V de tensão. Assim, optamos por um de 2.2mf e 100v para novamente garantir uma margem de erro |R$10 por 20 unidades|
|Diodo Zener   |1  | 13V - 1W | No geral, a corrente de pico (quando está em 3V) é aproximadamente 12 mA, o que resulta em uma voltagem de 156mW, mas o único diodo que conseguimos encontrar pra essa tensão (13V) foi este, então pelo menos temos, novamente, uma boa margem de erro|R$10,66 por 10 unidades|
|Resistência   | 1  | 680ohm  |   |   |
|Resistência    | 2   | 22ohm| Uma resistência foi utilizada para controlar a corrente que passa pelo NPN e não estora-lo e a outra representa o load|
|Resistência  | 1   | 3.1kohm    |    |
|Potenciômetro   |1   |   |   |   |


#### Link para o circuito no falstad
... (em construção)

#### Link para o vídeo explicativo
... (em construção)
