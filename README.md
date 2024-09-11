Previsão de Infecção pelo Vírus da AIDS Usando Modelos de Aprendizado de Máquina

##Descrição do Projeto
Este projeto visa desenvolver um modelo de aprendizado de máquina para prever a infecção pelo vírus da AIDS com base em características médicas e histórico de pacientes. Usando dados demográficos, históricos de tratamento e outros atributos médicos, criamos um modelo de classificação binária que pode ajudar a prever se um paciente está infectado ou não.

##Objetivo
O objetivo principal é construir um modelo preditivo que ofereça suporte na identificação de pacientes infectados pelo vírus da AIDS, utilizando atributos clínicos e demográficos.

##Conjunto de Dados
Os dados utilizados estão disponíveis em quatro arquivos CSV com diferentes quantidades de pacientes:
- AIDS_Classification.csv
- AIDS_Classification_5000.csv
- AIDS_Classification_15000.csv
- AIDS_Classification_50000.csv

Cada arquivo contém os seguintes atributos:

- Tempo (até falha ou censura),
- Tratamento,
- Idade, Peso,
- Histórico de uso de drogas, atividade homossexual,
- Classificação de Karnofsky,
- Contagem de células CD4/CD8,
- Raça, Gênero.

##Modelos Utilizados
O modelo principal escolhido para o projeto foi o Random Forest Classifier devido à sua robustez em lidar com variáveis categóricas e contínuas, além de sua capacidade de fornecer resultados precisos em problemas de classificação binária.

##Etapas do Projeto
1. Análise Exploratória de Dados (EDA):
   - Realização de uma análise exploratória para entender melhor a estrutura dos dados e identificar valores ausentes.
   - Identificação de variáveis categóricas e contínuas.
2. Pré-processamento dos Dados:
   - Tratamento de valores ausentes: Valores nulos foram substituídos pela mediana.
   - Codificação de variáveis categóricas: Variáveis como gênero e raça foram transformadas em variáveis dummy (one-hot encoding).
   - Normalização de variáveis contínuas: Variáveis como idade, peso e contagem de células foram normalizadas para melhorar o desempenho do modelo.
3. Treinamento do Modelo:
   - O modelo Random Forest foi treinado usando o conjunto de treino com validação usando um conjunto de teste.
   - Avaliamos o modelo usando as seguintes métricas
       - Acurácia
       - Sensibilidade (Recall)
       - Precisão
       - F1-Score
4. Avaliação do Modelo:
   - O modelo apresentou uma acurácia superior a 90%, com um bom equilíbrio entre precisão e recall.
   - Os resultados foram avaliados utilizando um relatório de classificação.
  
##Tecnologias Utilizadas
- Python 3.x
- Pandas: Manipulação de dados.
- Scikit-learn: Modelagem e avaliação do modelo.
- Gdown: Download de arquivos CSV do Google Drive.

##Como Executar o Projeto
1. Clone o repositório:
   git clone https://github.com/Cristina1607/previs-o-de-Infec-o-pelo-V-rus-da-AIDS.git
   cd previs-o-de-Infec-o-pelo-V-rus-da-AIDS
2. Instale as dependências necessárias:
   pip install -r requirements.txt
3. Execute o script de treinamento do modelo:
   python model_training.py

##Resultados
Os resultados finais indicam que o modelo Random Forest pode ser utilizado como uma boa ferramenta para prever a infecção pelo vírus da AIDS, com resultados precisos em diferentes tamanhos de conjunto de dados.

##Conclusões
O modelo apresentou bom desempenho com acurácia, precisão e recall elevados. Recomenda-se, no entanto, realizar ajustes nos hiperparâmetros e testar outros modelos de aprendizado de máquina para verificar se é possível melhorar ainda mais os resultados.

##Licença
Este projeto está licenciado sob a licença MIT - consulte o arquivo LICENSE para obter detalhes.
