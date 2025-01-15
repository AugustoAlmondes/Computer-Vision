# Treinamento de Rede Neural com Detectron2

Este repositório contém um projeto simples de treinamento de uma rede neural utilizando a biblioteca **Detectron2**. O objetivo é realizar a detecção de objetos para identificar gatos e cachorros em imagens.

## Descrição

O projeto aborda a implementação de um sistema de detecção de objetos usando a arquitetura **Faster R-CNN** como base, explorando as funcionalidades do Detectron2. A proposta é simples, mas envolve etapas essenciais para configurar e treinar o modelo, garantindo bons resultados de identificação.

### Principais etapas do projeto:
1. **Preparação do conjunto de dados**:
   - Utilização de dados obtidos do site **Roboflow**.
   - Divisão em conjuntos de treino, validação e teste.
   - Análise e pré-processamento das imagens e anotações.

2. **Configuração do modelo**:
   - Ajuste de hiperparâmetros (taxa de aprendizado, número de iterações, entre outros).
   - Escolha da arquitetura do modelo com base em pré-treinamento no Detectron2.

3. **Treinamento e avaliação**:
   - Testes realizados em cenários com diferentes classes e contextos (gatos isolados, cachorros isolados, e ambos juntos).
   - Uso de métricas como **loss total**, **false-negative**, e **cls-accuracy** para análise de desempenho.

## Resultados

Os testes demonstraram que o modelo foi capaz de:
- Detectar gatos e cachorros em imagens separadas.
- Identificar ambos os animais em uma mesma imagem.
- Apresentar bons resultados após ajustes nos hiperparâmetros e aumento no número de classes.

## Requisitos

Certifique-se de que os seguintes pacotes e bibliotecas estejam instalados no ambiente:
- **Python 3.8 ou superior**
- **PyTorch**
- **Detectron2**
- **TensorBoard** (para visualização de métricas)

## Execução

1. Clone este repositório:
   ```bash
   git clone https://github.com/AugustoAlmondes/Computer-Vision.git
   cd Computer-Vision
   ```
2. Instale as dependências necessárias.
3. Execute as células do notebook para configurar e treinar o modelo
4. Utilize o TensorBoard para visualizar métricas:
   ```bash
   tensorboard --logdir logs/
   ```
