# Projeto: Análise de Métricas de Classificação e Curva ROC

## Descrição do Projeto
Este projeto tem como objetivo realizar a análise de métricas de classificação e gerar a Curva ROC a partir de dados simulados. Ele utiliza bibliotecas como `numpy`, `pandas`, `matplotlib`, `seaborn` e ferramentas do `sklearn` para calcular métricas como Sensibilidade, Especificidade, Acurácia, Precisão, F-Score e AUC (Área sob a Curva).

O projeto também exibe uma matriz de confusão e realiza o plot da curva ROC para avaliar o desempenho de um classificador em distinguir entre classes positivas e negativas.

---

## Funcionalidades

- Cálculo das seguintes métricas de classificação:
  - Sensibilidade (Recall)
  - Especificidade
  - Acurácia
  - Precisão
  - F-Score
  - AUC (Área sob a Curva ROC)

- Exibição de uma matriz de confusão estilizada com `seaborn`.

- Plot da Curva ROC, incluindo a exibição do valor de AUC.

---

## Tecnologias Utilizadas

- **Python 3.8+**
- **Bibliotecas**:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `sklearn`

---

## Como Rodar o Projeto

### Pré-requisitos

1. Python instalado (versão 3.8 ou superior).
2. Instalar as dependências do projeto. Execute o comando:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```

### Execução

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```
2. Navegue até o diretório do projeto:
   ```bash
   cd seu-repositorio
   ```
3. Execute o script principal:
   ```bash
   python script_principal.py
   ```

---

## Estrutura do Código

- **`calcular_metricas`**:
  - Função que calcula métricas de classificação e os pontos necessários para a curva ROC.
- **`plotar_curva_roc`**:
  - Função responsável por gerar e exibir o gráfico da curva ROC.
- **Simulação de Dados**:
  - Os dados simulam probabilidades previstas para classes positivas e negativas (Utilizei dados menores, mas pode ser ajustado).

---

## Exemplo de Saída

### Métricas de Classificação
```plaintext
Sensibilidade (Recall): 0.91
Especificidade: 0.88
Acurácia: 0.90
Precisão: 0.85
F-score: 0.88
AUC (Área sob a Curva ROC): 0.93
```

### Matriz de Confusão

![Matriz de Confusão](#) <!-- Substitua com o caminho da imagem se salvar o gráfico como PNG -->

### Curva ROC

![Curva ROC](#) <!-- Substitua com o caminho da imagem se salvar o gráfico como PNG -->

---

## Personalização

Caso deseje utilizar dados reais em vez de simulados, substitua os arrays `true_labels` e `predicted_scores` por dados derivados de um modelo treinado ou de um dataset.

Exemplo:
```python
true_labels = [1, 0, 1, 1, 0, ...]  # Substitua pelos rótulos verdadeiros
predicted_scores = [0.8, 0.3, 0.9, 0.7, 0.2, ...]  # Substitua pelas probabilidades previstas
```

---

## Referências

- [Documentação do Scikit-learn](https://scikit-learn.org/stable/documentation.html)
- [Curvas ROC e Métricas de Classificação - Artigo Explicativo](https://en.wikipedia.org/wiki/Receiver_operating_characteristic)

---

## Autor

Desenvolvido por Wanderson Gustavo. Caso tenha dúvidas ou sugestões, entre em contato!

---

