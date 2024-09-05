![OrdemProducaoCapa](https://github.com/user-attachments/assets/9a966502-5281-4599-af2d-a09559b43c73)
# Análise de Dados de Produção - Previsão de Vida Útil Restante (RUL) com Random Forest
 
## Descrição do Projeto
Este projeto utiliza o algoritmo Random Forest Regressor para prever a Vida Útil Restante (RUL) de motores turbofan, baseado em dados de manutenção preditiva. O objetivo é estimar, com base em séries temporais multivariadas de sensores e parâmetros operacionais, o tempo restante até a falha de cada motor, permitindo uma estratégia de manutenção mais eficiente.

## Conjunto de Dados
Os dados utilizados no projeto estão disponíveis em arquivos de texto, fornecidos como parte de um desafio de manutenção preditiva. Cada arquivo contém séries temporais multivariadas com dados de operação de motores ao longo do tempo.
- Fonte dos dados: Kaggle - Predictive maintenance (https://www.kaggle.com/competitions/predictive-maintenance)
 - Colunas: O conjunto de dados contém 26 colunas, representando medições de sensores e configurações operacionais.
 - Arquivos:
   - train_FD001.txt: Dados de treinamento.
   - test_FD001.txt: Dados de teste.
   - RUL_FD001.txt: Vida útil restante real dos motores (utilizado para avaliação).
     
### Descrição dos arquivos
Conjunto de dados: FD001
Trjectórios de trem: 100 Trajetórias
de teste: 100
Condições: ONE (Nível do mar)
Modos de falha: ONE (Degradação de HPC)

Conjunto de dados: FD002
Trjectórios de trem: 260 Trajetórias
de teste: 259
Condições: SEIS
Modos de falha: UM (degradação de HPC)

Conjunto de dados: FD003
Trjectórios de trem: 100 Trajetórias
de teste: 100
Condições: UM (nível do mar)
Modos de falha: DOIS (degradação de HPC, degradação do ventilador)

Conjunto de dados: FD004
Trjectórios de trem: 248 Trajetórias
de teste: 249
Condições: SEIS
Modos de falha: DOIS (degradação de HPC, degradação do ventilador)

## Estrutura do Projeto
 - Projeto_Random_Forest.ipynb: Notebook com o código do projeto.
 - train_FD001.txt, test_FD001.txt, RUL_FD001.txt: Arquivos de dados utilizados no projeto.
 - README.md: Descrição do projeto.
 - requirements.txt: Lista de dependências necessárias para rodar o projeto.

## Objetivo
O objetivo deste projeto é desenvolver modelos para prever falhas em equipamentos e otimizar a manutenção preventiva.

## Resultados
O modelo foi treinado utilizando Random Forest Regressor, e os melhores parâmetros foram encontrados através de ajuste de hiperparâmetros com GridSearchCV. O desempenho do modelo foi avaliado utilizando o Root Mean Squared Error (RMSE), e o melhor valor de RMSE obtido foi de 41.8121.

## Instalação

### Requisitos
Para rodar este projeto, você precisará ter os seguintes pacotes instalados:
 - Pandas 
 - Numpy
 - Matplotlib 
 - Seaborn
 - Scikit-learn
 - Os

## Conclusão
Este projeto demonstrou a viabilidade da aplicação de algoritmos de aprendizado de máquina, como o Random Forest, na previsão de falhas e manutenção preditiva em motores turbofan. O uso de séries temporais multivariadas, aliado a uma robusta estratégia de ajuste de hiperparâmetros, resultou em um modelo preciso, com bom desempenho para prever a vida útil restante dos motores.
