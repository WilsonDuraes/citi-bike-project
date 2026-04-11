# 🚲 Estudo de Caso: Business Intelligence e Otimização Logística (Citi Bike NYC)

![Badge Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![Badge Data Analytics](https://img.shields.io/badge/Data_Analytics-000000?style=for-the-badge) ![Badge Logística](https://img.shields.io/badge/Otimização_Logística-0077B5?style=for-the-badge)

## 📌 O Contexto
A gestão de ativos espalhados geograficamente (como frotas, equipamentos ou sistemas de mobilidade) gera um volume massivo de dados transacionais. Este projeto utiliza o banco de dados real do sistema *Citi Bike* de Nova York (abrangendo anos de registros de APIs e AWS Athena) como laboratório para demonstrar a resolução de um gargalo logístico complexo.

## 🚨 O Problema (A Dor Operacional)
Como garantir que haja ativos disponíveis onde os clientes precisam e espaço livre onde eles precisam devolver? 

Lidar com mais de 50 arquivos CSV pesados contendo milhões de registros históricos (2016 a 2021) torna a análise em planilhas tradicionais (como o Excel) completamente inviável. Sem ferramentas adequadas de inteligência de dados, a diretoria fica "cega" operacionalmente: é impossível cruzar variáveis, prever horários de pico, identificar estações ociosas ou entender os gargalos da operação, resultando em perda de receita e insatisfação do cliente.

## 💡 A Solução 
Desenvolvimento de um pipeline analítico estruturado. A base massiva de dados brutos foi extraída, consolidada e limpa via código (tratando dados ausentes e convertendo formatos de sistema como Timestamps Unix). Em seguida, os dados de movimentação foram cruzados com variáveis externas (como condições climáticas) para realizar uma Análise Exploratória focada em **Inteligência de Negócio**.

## 📊 O Impacto e Aplicações (ROI)
Soluções analíticas como esta geram impactos diretos na operação de qualquer empresa de logística, distribuição ou gestão de frotas:
* **Visibilidade Gerencial:** Transformação de milhões de linhas ilegíveis em respostas claras sobre a operação diária.
* **Redução de Custos e Eficiência:** A identificação de padrões climáticos e de horário permite alocar equipes de remanejamento de frota apenas para onde e quando realmente há demanda, otimizando recursos físicos e humanos.
* **Escalabilidade Analítica:** Capacidade de processar e analisar 5 anos de dados históricos em segundos, superando as limitações dos softwares comuns de escritório.

## 🛠️ Stack Tecnológico Utilizado
* **Linguagem Base:** `Python`
* **Processamento Massivo:** `Pandas` e `NumPy` (Manipulação, limpeza e consolidação de múltiplos arquivos CSV e dados estruturados).
* **Análise Visual:** `Matplotlib` e `Seaborn` (Geração de relatórios visuais e identificação de padrões).
* **Origem dos Dados:** Manipulação de extrações via API e *AWS Athena*.

---
*Desenvolvido por **Wilson Durães** | Consultor de Dados, Automação e Inteligência Gerencial*
* [Conecte-se comigo no LinkedIn](https://www.linkedin.com/in/wilsonduraes)
