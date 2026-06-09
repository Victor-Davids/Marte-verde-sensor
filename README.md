# Marte-verde-sensor

Descrição do projeto

Sensor que avalia o local atraves de 5 criterios sendo: solo, temperatura, humidade, pressão do ar e radiação. Para determinar se pode ser usado para plantio.

Objetivo da solução

Seu principal objetivo e observa e registrar o ambiente das cavernas de marte para se tornaram futuras bases de plantio para a humanidade tornando o gigante vermelho um planeta habitavel e autosufisiente num futuro distante.

Componentes utilizados

Arduino UNO x 1
DHT 22 x 1
BMP-180 x 1
Potenciometro x 1
HC-SR04 x 1
Breadboard x 1

Explicação do funcionamento

HC-SR04 emite um pulso que age como um ultrassonico, quando este pulso volta ele analisa se a onda encontrou agua, e caso tenha encontrado, emite um alerta.
BMP-180 faz a leitura da pressão do ar, potenciometro atua como um radiador e mede a radiação com o maximo do indice uv chegando a 11.0 e o DHT por padrão faz a leitura da humidade e temperatura. Todas essas informações são compiladas e enviadas com adicional de se o nível do radar indicar presença de água (faixa estabelecida de 15 a 30) e o indice UV estiver baixo (menor que 3.0), o sistema valida o local como seguro para o cultivo. Caso contrário, ele dispara alertas de solo seco ou radiação nociva. 

Estrutura do circuito Instruções de execução

As conexões elétricas devem ser distribuídas da seguinte forma nos pinos do Arduino:

Sensor Ultrassônico HC-SR04
VCC - Pino 5V do Arduino
TRIG - Pino Digital 9 do Arduino
ECHO - Pino Digital 8 do Arduino
GND - Pino GND do Arduino

Sensor BMP180
VCC - Pino 3.3V (ou 5V dependendo do módulo) do Arduino
GND - Pino GND do Arduino
SCL - Pino Analógico A5 do Arduino (ou pino SCL dedicado)
SDA - Pino Analógico A4 do Arduino (or pino SDA dedicado)

Sensor DHT22
VCC - Pino 5V do Arduino
DATA - Pino Digital 2 do Arduino
GND - Pino GND do Arduino

Potenciometro
VCC - Pino 5V (ou 3.3V dependendo do módulo) do Arduino
OUT - Pino Analógico A0 do Arduino
GND - Pino GND do Arduino

conecte as entradas GND, V5 e v3.3 do arduino nas pontas do breadboard depois disso faça a coneção dos componentes em seus respectivos lugares dando um pouco de espaço e copie o codigo de C++ deste github.
lembrece da baixar as bibliotecas para o funcionamento correto.
RM571973 - Victor David
