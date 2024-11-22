# Synergy-Edge-Computing
A solução proposta pela Synergy utiliza tecnologias modernas para resolver o desafio do consumo energético ineficiente nas indústrias. Nossa abordagem combina hardware de alta eficiência, como a plataforma ESP32, com sensores/atuadores inteligentes e comunicação HTTP, para oferecer um sistema integrado de monitoramento e controle.

Ao capturar dados em tempo real sobre o consumo de energia de máquinas e equipamentos, nossa solução permite que gestores industriais identifiquem desperdícios e implementem ações corretivas rapidamente. Além disso, com a integração de métodos de comunicação robustos, como HTTP para armazenamento e visualização de dados, conseguimos criar um ecossistema eficiente e flexível.

Resumo da Implementação Técnica
Plataforma ESP32 e Sensores:

O ESP32 é responsável por capturar dados de sensores simulados no ambiente Wokwi. Sensores como potenciômetros representam consumo energético, enquanto atuadores podem ser usados para responder a comandos.
Comunicação HTTP:

Dados capturados pelo ESP32 são enviados via HTTP para um servidor Flask, que se comunica com o Orion Context Broker (FIWARE). Isso permite o armazenamento e consulta de dados.
Integração com o Orion Context Broker (FIWARE):

Os dados são enviados do servidor Flask para o Orion, onde são gerenciados e disponibilizados para consultas e integrações futuras, como visualização em dashboards ou análise preditiva.
Resumo das Implementações Feitas
Simulação no Wokwi:
Criamos um código no ESP32 que simula sensores de corrente e potência, enviando dados para o servidor Flask.
Servidor Flask:
Desenvolvemos endpoints que recebem dados do ESP32, armazenam no FIWARE (Orion Context Broker) e permitem consultas.
Orion Context Broker:
Configuramos o Orion para gerenciar os dados de consumo energético, com suporte para consultas e armazenamento.
