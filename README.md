# Dispenser Automatico de Ração
Aqui neste repositório contém as informações e código referente ao projeto da Aula 4 de Objetos Integrados

O funcionamento será da seguinte forma, o arduino irá conter dentro de seu loop um timer, onde sempre que termina a contagem, será acionado o servomotor para que tenha uma abertura suficiente para uma breve vazão da ração, que irá cair diretamente no pote do animal, sendo interrompida a vazão logo em seguida, após isso, deve ser analisado os sinais do sensor ultrassônico, que será posicionado no topo do recipiente de ração, onde, conforme mais distante ele detectar a ração do fundo do recipiente, menor será a porcentagem de preenchimento do mesmo, e então será enviado a mensagem para o Broker do MQTT com informações referentes ao preenchimento desse recipiente, através do MQTT, é possível também enviar um sinal para que seja realizado a abertura manual do dispenser do recipiente, dessa forma, podendo despejar mais ração com antecedência.

##Hardware utilizados no projeto:
Esses foram os hardware que foram utilizados ao longo do projeto, vocÊs podem estar comprando do estabelecimento e marca que melhor encaixarem no seus bolsos.

* Arduino Uno
* Ethernet Shield W5100
* Protoboard
* Servo Motor
* Sensor de Distância Ultrassônico HC-SR04
* Cabo Jumper
* Cabo USB-AB
* Adaptador de Energia

##Documentação das interfaces, protocolos e módulos de comunicação utilizados no projeto:
Essas são as documentações utilizadas para guiar o código do projeto ao funcionamento do hardware.

* [Node-Red](https://nodered.org/docs/)
* [Firmata](https://github.com/firmata/protocol)
* [Arduino IDE](https://docs.arduino.cc/)

##Comunicação/controle via internet (TCP/IP) e uso do Protocolo MQTT:
Ferramentas utilizadas para que fosse possivel a comunicação com internet e utilização do MQTT.

* [Aedes Broker](https://flows.nodered.org/node/node-red-contrib-aedes)
* [MQTTBox](https://chrome.google.com/webstore/detail/mqttbox/kaajoficamnjijhkeomgfljpicifbkaf?hl=pt-BR)
