# Projeto: Transfer Learning em Python com Deep Learning

## Descrição

Este projeto aplica o método de Transfer Learning utilizando redes de Deep Learning em Python no ambiente Google Colab. O objetivo é classificar imagens em duas classes distintas ("Dog" e "Cat") a partir de um dataset de imagens. A solução implementa ajustes nas últimas camadas de um modelo pré-treinado para adaptar-se à tarefa proposta, mesmo com um conjunto de dados reduzido.

Este projeto utiliza o dataset "Cats vs. Dogs" disponibilizado pela Microsoft Research, mas permite o uso de outras bases de dados personalizadas.

## Dataset

- **Fonte do Dataset**: [Cats vs. Dogs TensorFlow](https://www.tensorflow.org/datasets/catalog/cats_vs_dogs)
- **Download do Dataset**: [Microsoft Research](https://www.microsoft.com/en-us/download/details.aspx?id=54765)
- **Estrutura**: Imagens divididas em duas classes - "Dog" e "Cat".

**Observação:**
Você pode substituir o dataset por uma base de dados personalizada com duas classes de sua escolha.

## Funcionalidades

- Carregamento e limpeza do dataset.
- Divisão do dataset em conjunto de treinamento, validação e teste (70%, 15%, 15%).
- Normalização e pré-processamento das imagens.
- Utilização de Transfer Learning para criar um classificador personalizado.
- Visualização de resultados através de métricas de perda e acurácia.
- Predições baseadas em imagens fornecidas pelo usuário.

## Tecnologias Utilizadas

- **Linguagem**: Python
- **Frameworks**:
  - TensorFlow / Keras
  - Matplotlib
  - OpenCV
- **Ambiente**: Google Colab

## Requisitos

**Bibliotecas Necessárias:**
- `tensorflow`
- `keras`
- `opencv-python`
- `numpy`
- `matplotlib`
- `google.colab`

Para instalar as dependências, execute:
```bash
pip install tensorflow keras opencv-python matplotlib
```

## Estrutura do Projeto

### Carregamento do Dataset
- Limpeza de arquivos inválidos.
- Redimensionamento das imagens para 224x224 pixels.
- Rótulos binários atribuídos ("Dog": 0, "Cat": 1).

### Divisão do Dataset
- **Treinamento**: 70%
- **Validação**: 15%
- **Teste**: 15%

### Treinamento do Modelo
- Utilização de uma arquitetura pré-treinada (ex: VGG16 ou similar).
- Ajuste das últimas camadas do modelo.

### Avaliação do Modelo
- Gráficos de validação (perda e acurácia).
- Métricas de desempenho no conjunto de teste.

### Predição
- Classe prevista e probabilidade associada para uma nova imagem fornecida.

## Como Executar

### Passo 1: Configuração do Ambiente

Suba o projeto no Google Colab.

Conecte seu Google Drive para acessar o dataset:
```python
from google.colab import drive
drive.mount('/content/drive')
```

### Passo 2: Carregue e Pré-processar o Dataset
Certifique-se de que as imagens estão organizadas no caminho definido:
```python
base_dir = '/content/drive/MyDrive/PetImages'
```

### Passo 3: Treinamento do Modelo
Execute as etapas de treinamento e ajuste fino do modelo. Os gráficos e métricas de desempenho serão gerados automaticamente.

### Passo 4: Predições
Forneça o caminho de uma imagem para predizer a classe:
```python
img, x = get_image('/path/to/your/image.jpg')
probabilities = model_new.predict([x])
```

## Resultados

- **Acurácia no Conjunto de Teste**: Relatado após a avaliação.
- **Gráficos**: Visualização de perda e acurácia durante o treinamento.
- **Predições**: Exemplo:
  - Classe prevista: Dog
  - Probabilidade: 0.85

## Observações Importantes

- Garanta que todas as imagens estejam limpas antes do treinamento.
- Use um dataset balanceado para melhorar o desempenho do modelo.
- Ajuste o hiperparâmetro `max_images_per_class` para controlar a quantidade de dados usada.

## Contribuições

Contribuições são bem-vindas! Envie um Pull Request ou abra uma Issue para discutir melhorias.

## Licença

Este projeto é licenciado sob a [MIT License](LICENSE).
