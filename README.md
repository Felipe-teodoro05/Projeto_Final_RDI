# Projeto_Final_RDI
Realizado por:
- Felipe Teodoro
- Jamille Rocha
- Pedro Aragão
- Manuella Borges
- Henrique Valle

# Utilizando Scrapy para raspar dados da OLX

## Descrição do Projeto

Este projeto utiliza o framework **Scrapy** para realizar a raspagem de dados de anúncios de carros na plataforma OLX. A ferramenta Scrapy é altamente eficiente para coletar dados estruturados de websites de forma automatizada e escalável. O foco deste projeto é extrair informações de anúncios de carros, como título, preço e localização, da seção de **Carros e Eletrodomésticos** da OLX.

As seguintes etapas foram implementadas:

1. **Configuração da aranha**: 
   - Utilização de um `USER_AGENT` customizado para imitar um navegador legítimo e evitar bloqueios pelo site.
   - Ativação do **AutoThrottle** para ajustar automaticamente a velocidade das requisições, minimizando a sobrecarga do servidor e o risco de bloqueio.

2. **Raspagem de várias páginas**: 
   - O método `start_requests` faz requisições para as primeiras 100 páginas do site OLX.
   - Processamento paralelo das páginas para otimizar o tempo de execução.

3. **Extração de dados**:
   - Utilização de **XPath** para acessar a estrutura JSON da página OLX e extrair os seguintes dados:
     - **Título**: Nome do carro
     - **Preço**: Preço do carro
     - **Localização**: Localização do anúncio

4. **Armazenamento dos dados**:
   - Os dados coletados são salvos em um arquivo **JSON**, permitindo uma análise futura dos anúncios extraídos.
  

# **Parte de Análise de Dados do Data Hackers 2023**:
   O segundo projeto envolve a análise exploratória de um dataset do **Data Hackers 2023**, publicado no Kaggle. A análise inclui visualizações sobre idade, etnia, área de formação, salário e outras características de profissionais da área de dados.

A junção desses dois projetos permite uma visão completa tanto de dados de um site como a OLX quanto de uma análise mais detalhada sobre o mercado de trabalho na área de dados, com insights sobre diversidade, salários, cargos e modelos de trabalho.


## Instruções para Execução

1. **Instale as dependências**:

   Certifique-se de ter o Python instalado em sua máquina. Para instalar as dependências necessárias, execute o seguinte comando:

   ```bash
   pip install -r requirements.txt
