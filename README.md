# Análise de Mobilidade Urbana com Dados do Citi Bike em Nova York

## Contexto do Estudo

O Citi Bike é um sistema de compartilhamento de bicicletas em Nova York, operado pela Motivate e financiado pela empresa de transporte público da cidade. O objetivo deste projeto é analisar os dados do Citi Bike para entender padrões de uso, avaliar a disponibilidade de bicicletas e otimizar a distribuição nas estações.

## Referências de Aquisição do Dataset

- **Fonte dos Dados**: [Citi Bike Stations Dataset](https://www.kaggle.com/datasets/rosenthal/citi-bike-stations)
- **Descrição**: O dataset contém informações sobre as estações do Citi Bike, incluindo a disponibilidade de bicicletas e docas, a localização das estações e a capacidade de cada estação.
- **Período da Coleta**: (Inclua o período de coleta dos dados, se disponível.)

## Descrição da Origem

O Citi Bike é um sistema de bicicletas compartilhadas que fornece um meio de transporte sustentável para residentes e visitantes de Nova York. Os dados foram coletados das estações do Citi Bike e refletem a disponibilidade de bicicletas e docas, status das estações e informações de localização.

## Descrição do Dataset

O dataset contém as seguintes colunas:

- **station_id**: Identificador único da estação (ex.: 3195).
- **num_bikes_available**: Número de bicicletas disponíveis na estação (ex.: 25).
- **num_ebikes_available**: Número de bicicletas elétricas disponíveis na estação (ex.: \N para dados ausentes, 0 para nenhuma bicicleta elétrica disponível).
- **num_bikes_disabled**: Número de bicicletas fora de serviço na estação (ex.: \N para dados ausentes, 0 para nenhuma bicicleta fora de serviço).
- **num_docks_available**: Número de docas disponíveis na estação (ex.: 13).
- **num_docks_disabled**: Número de docas fora de serviço na estação (ex.: \N para dados ausentes, 1 para uma doca fora de serviço).
- **is_installed**: Se a estação está instalada (1) ou não (0) (ex.: 1).
- **is_renting**: Se a estação está disponível para aluguel (1) ou não (0) (ex.: 1).
- **is_returning**: Se a estação está disponível para devolução (1) ou não (0) (ex.: 1).
- **station_status_last_reported**: Data e hora do último relatório de status da estação, representado como um timestamp Unix (ex.: 1547045888).
- **station_name**: Nome da estação (ex.: Montgomery St).
- **lat**: Latitude da estação (ex.: 40.71942).
- **lon**: Longitude da estação (ex.: -74.05099).
- **region_id**: Identificador da região onde a estação está localizada (ex.: 70).
- **capacity**: Capacidade total da estação, ou seja, o número máximo de bicicletas e docas (ex.: 14).
- **has_kiosk**: Se a estação possui um quiosque (1) ou não (0) (ex.: true).
- **station_information_last_updated**: Data e hora da última atualização das informações da estação, representado como um timestamp Unix (ex.: 1564692450).
- **missing_station_information**: Se há informações faltando sobre a estação (1) ou não (0) (ex.: false).


## Objetivos do Projeto

- **Analisar a Disponibilidade de Bicicletas**: Investigar como a disponibilidade de bicicletas varia ao longo do tempo.
- **Avaliar a Influência Climática**: Estudar como as condições climáticas afetam a disponibilidade e o uso das bicicletas.
- **Otimizar a Distribuição de Bicicletas**: Propor melhorias para a gestão e distribuição das bicicletas e docas nas estações.

## Metas e Milestones

- **Etapa 1**: Identificação e Coleta dos Dados - Completa.
- **Etapa 2**: Definição do Objetivo do Estudo - Completa.
- **Etapa 3**: Preparação e Organização dos Dados - Em Andamento.
- **Etapa 4**: Análise Exploratória dos Dados - A Ser Iniciada.
- **Etapa 5**: Elaboração da Proposta Analítica - A Ser Iniciada.
- **Etapa 6**: Consulta com o Professor - A Ser Agendada.

## Cronograma

- **Semana 1-2**: Coleta e preparação dos dados.
- **Semana 3-4**: Análise exploratória e visualização dos dados.
- **Semana 5-6**: Desenvolvimento de modelos analíticos e interpretação dos resultados.
- **Semana 7-8**: Elaboração do relatório final e preparação da apresentação.

## Link para o Repositório do Projeto

O código e os materiais relacionados ao projeto estão disponíveis no [GitHub do Projeto](https://github.com/WilsonDuraes/citi-bike-project).

---

*Para qualquer dúvida ou feedback, entre em contato através dos canais de comunicação disponíveis.*

