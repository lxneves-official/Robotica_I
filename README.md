# Aula 05

Controlar o acendimento de um LED com a LUZ.

## Introdução:

Você já percebeu que quando escurece os postes como num passe de mágica acende? Será que é mágica ou existe um funcionário da prefeitura que quando anoitece aciona um botão e as luzes acendem? Nada disso! existem alguns sensores que trabalham de acordo com a intensidade de luz, como por exemplo o LDR. Aqui você poderá controlar uma rua com postes de LED neste experimento com o LDR.

## Tarefa:

Utilizar um Sensor LDR para controlar o funcionamento de um LED.

## Recursos:

* Um computador.
* Um Arduino Uno R3.
* Cabo USB para Arduino.
* LED
* Sensor LDR
* Resistor 220 Ohms (vermelho, vermelho, marrom, dourado)

<div align="center">
<img src="https://github.com/user-attachments/assets/186bc1c9-d0b9-43a8-8e82-e1128ac69bab" alt="1 resistor" style="width: 20%; height: auto;">
</div>
  
* Resistor 10k Ohms (marrom, preto, laranja, dourado)

<div align="center">
<img src="https://github.com/user-attachments/assets/8636ff68-4878-4ee4-92a5-3f581a1ca410" alt="1 resistor" style="width: 20%; height: auto;">
</div>

## Processo:

* Faça a montagem do circuito abaixo:

<div align="center">
<img src="https://github.com/user-attachments/assets/23146165-ec9c-4796-af2d-caab33ae5e29" alt="1 resistor" style="width: 60%; height: auto;">
</div>

* Abra o programa Arduino IDE;
* Na nova sketch, limpe as linhas de comentários e deixe apenas o código válido ( **_void setup() e void loop ()_** );
* Antes do **_void setup()_** declare uma variável inteira (_int_) com o nome _ValorSensor_ e atribua o valor zero para esta variável;
  
      int ValorSensor = 0;
  
* Dentro do **_void setup()_** configure o Modo do pino _A0_ como entrada de sinal _INPUT_ e inicialize o monitor serial com a função _Serial.begin(115200)_;
* Dentro do **_void loop()_** atribua a variável _ValorSensor_ a informação lida pela porta _A0_ utilizando a função **_AnalogRead(A0)_**;
* Utilize a função _Serial.print_ para mostar no monitor serial o valor lido pelo sensor;
* Utilize a função _delay()_ para criar uma pausa de 0,5 segundo antes de fazer a próxima leitura;
* Execute o código;
* Cubra o Sensor com as mãos e veja o que ocorre com os valores apresentados no monitor serial;


* A função _if_ possui a seguinte sintaxe:

      if (condição)
      {
      
      }

* A condição deve ser a variável _ValorSensor_ de modo que o _if_ somente será executado se a variável ultrapassar um determinado valor;
* Dentro desse _if_ deve ser realizado o acionamento do LED utilizando a função **_digitalWrite ()_**;
* Se a montagem estiver igual a sugerida anteriormente o LED deve estar ligado na porta 9;

## Desafio

* Implemente o código para que o LED acenda quando a luminosidade obtida pelo sensor diminua, escolha um valor.

## Registro

* Faça um relatório dessa atividade utilizando o modelo disponibilizado no Classroom.
* Após finalizar a montagem e obter a validação do professor, faça o registro fotográfico do circuito desenvolvido e um vídeo apresentando o funcionamento do circuito.
* Adicione o registro dessa atividade e o relatório desenvolvido no seu portfólio e entregue o link do portfólio publicado na atividade do **Classroom**.

