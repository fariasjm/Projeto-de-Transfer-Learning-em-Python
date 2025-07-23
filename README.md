# Projeto de Transfer Learning em Python

## Objetivo
Demonstrar o uso de Transfer Learning em um problema de classificação de imagens, aplicando ajustes em um modelo pré-treinado para adequá-lo ao conjunto de dados utilizado.

## Etapas do Projeto

01. Preparação dos Dados
  - Utilização do dataset Cats vs Dogs fornecido pelo TensorFlow Datasets (TFDS).
  - Preprocessamento das imagens:
    - Redimensionamento para 64x64 pixels.
    - Normalização dos valores dos pixels.
    - Conversão de rótulos para formato one-hot.

02. Divisão do Dataset
  - Separação dos dados em conjuntos de treino, validação e teste (70%, 15%, 15% respectivamente).
  - Organização em lotes para otimização do treinamento.

03. Modelo Utilizado
  - Base: VGG16 pré-treinada no ImageNet.

04. Treinamento do Modelo
  - Configuração:
    - Função de perda: categorical_crossentropy.
    - Otimizador: Adam.
    - Métrica: acurácia.
  - Treinamento em 10 épocas com batch size de 128.
  - Avaliação em dados de validação.

05. Avaliação e Resultados
  - Análise das métricas de desempenho (perda e acurácia) em gráficos para entender o comportamento do modelo ao longo das épocas.





