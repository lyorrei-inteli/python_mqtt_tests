# Simulador de Dispositivos IoT - Testes

Este repositório contém um simulador de dispositivos IoT para sensor de radiação solar e um conjunto de testes automatizados para validar o simulador.

## Como instalar

Após clonar o repositório, navegue até a pasta do projeto e instale as dependências necessárias:

```bash
pip install -r requirements.txt
```

## Como rodar o sistema

Para iniciar o simulador, execute o seguinte comando:

```bash
python3 publisher.py
```

Para iniciar o subscriber que irá ouvir as mensagens publicadas pelo simulador, abra um novo terminal e execute:

```bash
python3 subscriber.py
```

## Executar os Testes

Para executar os testes automatizados, use o seguinte comando:

```bash
pytest tests/
```

## Demonstração do Sistema

Demonstração dos Publishers e Subscribers: [Link do vídeo](https://youtu.be/mvigfNvgJ_4) <br/>
Demonstração dos testes: [Link do vídeo](https://youtu.be/P0oVfgMh7zs)

## Estrutura do Projeto

- `publisher.py`: Contém o código do publicador que envia dados simulados de um sensor de radiação solar para um broker MQTT.
- `subscriber.py`: Contém o código do assinante que escuta e imprime as mensagens do tópico MQTT.
- `sensor_simulator.py`: Define a classe `SolarRadiationSensorSimulator` que simula dados de radiação solar.
- `tests/`: Pasta contendo os testes automatizados para o simulador.
  - `test_sensor_simulator.py`: Testes automatizados para validar as funcionalidades do simulador.
