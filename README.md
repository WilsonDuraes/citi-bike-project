# Análise de Mobilidade Urbana com Dados do Citi Bike em Nova York

## Contexto do Estudo

O Citi Bike é um sistema de compartilhamento de bicicletas em Nova York, operado pela Motivate e financiado pela empresa de transporte público da cidade. O objetivo deste projeto é analisar os dados do Citi Bike para entender padrões de uso, avaliar a disponibilidade de bicicletas e otimizar a distribuição nas estações.

## Sobre o Dataset

O Citi Bike de Nova York possui uma API pública em tempo real que segue a Especificação Geral de Feed de Compartilhamento de Bicicletas. Esta API contém informações sobre o número de bicicletas e docas disponíveis em cada estação de NYC.

Desde 2016, a API pública foi consultada a cada 2 minutos e os resultados foram armazenados. Este dataset contém todos esses resultados, desde 15/08/2016 até 08/12/2021. Os dados estão disponíveis no formato CSV, que pode não ser ideal para grandes volumes de dados, mas é um formato universalmente aceito. Para análises extensivas, recomenda-se converter os CSVs para formatos como parquet.

Em 2019, foi feita uma atualização para consultar a API através de uma função Lambda e também começou-se a consultar a API de informações das estações semanalmente para coletar dados sobre cada estação, como nome, latitude e longitude. No entanto, os dados de informações das estações estão ausentes entre 2016 e 08/2019. É possível preencher esses dados com as informações mais antigas disponíveis para cada estação, embora isso não garanta precisão.

## Detalhes do Dataset

- **Arquivos CSV**: O dataset está dividido em 50 arquivos CSV, cada um contendo dados históricos para um determinado `station_id`. As estações são distribuídas aleatoriamente entre esses arquivos para reduzir o tamanho individual dos arquivos.
- **Informações de Estações**: As informações das estações estão ausentes para dados anteriores a 08/2019. A coluna `missing_station_information` indica quando essas informações estão faltando. As informações da estação são precisas dentro de um período de 7 dias antes da atualização mais recente.
- **Formato dos Dados**: Os arquivos CSV foram gerados por uma consulta `CREATE TABLE AS` no AWS Athena usando o formato TEXTFILE. Portanto, valores nulos são demarcados como `\N`. As colunas de timestamp, `station_status_last_reported` e `station_information_last_updated`, estão em unidades de tempo POSIX/UNIX (segundos desde 1970-01-01 00:00:00 UTC).

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

