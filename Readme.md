# Projeto de Integração de Sistemas Informáticos (ISI)

## Feito por: Fábio Rodrigues Ferreira a29365 LESI 2026/27

**_Análise e Otimização de Dados para Sugestões de Alojamento Local_**

Repositório e projeto desenvolvido no âmbito da unidade curricular de **Integração de Sistemas Informáticos** da Licenciatura em Engenharia de Sistemas Informáticos na **UPCA**.

---

## Como Executar o Projeto

Para testar e visualizar o dashboard e o mapa interativo, o projeto recorre a contentorização com Docker.

### Pré-requisitos

- Ter o [Docker Desktop](https://www.docker.com/) instalado e a correr no computador.
- Ligação à internet para que o Node-RED consiga aceder ao cluster MongoDB Atlas e à API OpenWeatherMap.

### Passos para Execução

1. Abrir o terminal na pasta raiz deste projeto.
2. Executar o comando para iniciar o contentor Node-RED:

   docker compose up -d

3. No Node-RED, importar flows.json da pasta src/ para ter o fluxo completo

### Tecnologias Utilizadas

KNIME Analytics Platform - Processamento ETL, transformação de dados, e regras iniciais.

## Aviso do KNIME: Reconheço que não encontrei nenhuma forma de criar um caminho relativo para os ficheiros de input.
##                 por favor ver isso nos CSV e XML readers

MongoDB Atlas Cluster - Base de dados NoSQL na nuvem para persistência dos alojamentos e freguesias.

Node-RED & Docker - Orquestração do dashboard, automação horária de pedidos meteorológicos por API e renderização do mapa interativo.

### Organização das pastas

tp01a29365/
│
├── README.md                 > Descrição do projeto e instruções de execução
├── docker-compose.yml        > Ficheiro de orquestração para levantamento do contentor Node-RED
│
├── BD/                       > Ficheiros de exportação da base de dados
├── data/                     > Ficheiros de dados brutos e suporte
├── dataintegration/          > Ficheiro com as transformações, metanodes e jobs desenvolvidos no KNIME
├── doc/                      > Relatório final do projeto em formato PDF
├── nodered_data/             > Volume persistente para salvaguarda dos fluxos e configurações do Node-RED
├── src/                      > Contém flows.json, para correr no Node-RED

### Link do video de demonstração

https://alunosipca-my.sharepoint.com/:v:/g/personal/a29365_alunos_ipca_pt/IQCMDJ6o_rf2TK6mM_Dl7axZAXLRe8lnGzeZPEebToGrykE?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=rQSy0q
