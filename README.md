
ChiTu: Carro Inteligente
Uma extensão MakeCode para programar um carro inteligente educacional.

Diagrama de Fiação
O diagrama será exibido em breve.

Motor
Controle o Chitu para ir para frente, para trás, virar à esquerda e virar à direita.

Controlar o carro para frente


chitu.motorRun(chitu.Motors.M1, chitu.Dir.CW, 120)
chitu.motorRun(chitu.Motors.M2, chitu.Dir.CW, 120)
Controlar o carro para trás

chitu.motorRun(chitu.Motors.M1, chitu.Dir.CCW, 120)
chitu.motorRun(chitu.Motors.M2, chitu.Dir.CCW, 120)
Controlar o carro para virar à esquerda


chitu.motorRun(chitu.Motors.M1, chitu.Dir.CCW, 80)
chitu.motorRun(chitu.Motors.M2, chitu.Dir.CW, 120)
Controlar o carro para virar à direita


chitu.motorRun(chitu.Motors.M1, chitu.Dir.CW, 120)
chitu.motorRun(chitu.Motors.M2, chitu.Dir.CCW, 80)
Parar o motor esquerdo do Chitu


chitu.motorStop(chitu.Motors.M1)
Parar o motor direito do Chitu


chitu.motorStop(chitu.Motors.M2)
Parar os motores esquerdo e direito do Chitu


chitu.motorStop(chitu.Motors.All)
Servo

Definir o servo1 do Chitu para 90°


chitu.servoRun(chitu.Servos.S1, 90)
Definir o servo2 do Chitu para 120°


chitu.servoRun(chitu.Servos.S2, 120)
Ler sensor de linha

Ler o sensor de linha esquerdo


serial.writeNumber(chitu.readPatrol(chitu.Patrol.PatrolLeft))
Ler o sensor de linha do meio


serial.writeNumber(chitu.readPatrol(chitu.Patrol.PatrolMiddle))
Ler o sensor de linha direito


serial.writeNumber(chitu.readPatrol(chitu.Patrol.PatrolRight))
Evento do sensor de linha

Quando o sensor de linha esquerdo está em alta


chitu.ltEvent(chitu.Patrol1.PatrolRight, chitu.Voltage.High, function () {
    serial.writeNumber(1)
})
Quando o sensor de linha esquerdo está em baixa


chitu.ltEvent(chitu.Patrol1.PatrolRight, chitu.Voltage.Low, function () {
    serial.writeNumber(0)
})
Luzes LED

Ligar a luz LED esquerda


chitu.writeLED(chitu.LED.LEDLeft, chitu.LEDswitch.turnOn)
Desligar a luz LED esquerda

chitu.writeLED(chitu.LED.LEDLeft, chitu.LEDswitch.turnOff)
Ligar a luz LED direita


chitu.writeLED(chitu.LED.LEDRight, chitu.LEDswitch.turnOn)
Desligar a luz LED direita

chitu.writeLED(chitu.LED.LEDRight, chitu.LEDswitch.turnOff)
Licença MIT

Alvos suportados para PXT/microbit
* for PXT/microbit
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
