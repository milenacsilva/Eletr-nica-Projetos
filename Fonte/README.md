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
|Transformador   |1  | 127 – 220VAC (bivolt) 12V + 12V – 500mA  | Nosso intuito com esse componente era transformar de 127 Vac para 24 Vac garantir uma marge grande de erro para as quedas de tensão nos componentes. Além disso, o 12V + 12V é um ótimo custo benefício |R$21,90 |
|Diodo Retificador   |4  | 1N5408 | O diodo necessário era de aproximadamente 25V de tensão de pico e 500mA (obtidos a partir da saída do transformador). No entanto, optamos por um de 1000V e 3A ao baixo valor utilidade, garantindo uma ainda maior margem de erro ( esse definitiamente não vai queimar :) )   | R$2,40 por 10 unidades |
|Capacitor   |1 | 2.2mf 100v  |Utilizando a fórmula C = (amperagem [mili amperes] * tempo [mili segundos])/voltagem [volts], calculamos que a  capacitancia necessária será 2.075 mF com 25V de tensão. Assim, optamos por um de 2.2mf e 100v para novamente, garantir uma margem de erro |R$10 por 20 unidades|
|Diodo Zener   |1  | 13V - 1W | No geral, a corrente de pico (quando essa está em 3V) é aproximadamente 12 mA, o que resularia numa voltagem de 156mW, mas o único diodo que conseguimos encontrar pra essa tensão (13V) foi esse então pelo menos temos, novemente uma grande margem de erro|R$10,66 por 10 unidades|
|Resistencia 680ohm  | 1  |   |   |   |
|Resistencia  22ohm  | 2   | Uma foi utilizada para controlar a corrente que passa pelo NPN e não estora-lo e a outra representa o load| |
|Resistencia 3.1kohm | 1   |     |    |
|Potenciometro   |1   |   |   |   |


#### Link para o circuito no falstad
... (em construção)

#### Link para o vídeo explicativo
... (em construção)
