# Regressão Linear — Kit de Estudos

Este repositório contém um notebook Jupyter com um exemplo didático de **Regressão Linear**.
O objetivo é mostrar, passo a passo, como definir dados, ajustar um modelo simples,
calcular métricas e visualizar o resultado.

## Conteúdo
- Definição dos vetores de entrada **X** e saída **y**.
- Ajuste da reta com `numpy.polyfit` (sem dependências externas).
- Cálculo de métricas: **R²**, **MSE** e **MAE**.
- Gráfico com dados observados e reta ajustada.
- Exemplo de **previsão** para um novo valor (x = 6).

## Como executar
1. Abra o notebook `RegressaoLinear_comentado_avaliado.ipynb` no Jupyter/Colab/VsCode.
2. Execute as células na ordem.
3. Opcionalmente, altere os vetores `X` e `y_arr` para experimentar outros dados.

## Fórmulas das métricas
- **MSE** (Mean Squared Error): MSE = (1/n) * Σ (y_i − ŷ_i)^2  
- **MAE** (Mean Absolute Error): MAE = (1/n) * Σ |y_i − ŷ_i|  
- **R²** (Coeficiente de determinação): R² = 1 − (SS_res / SS_tot)  
  - SS_res = Σ (y_i − ŷ_i)^2  
  - SS_tot = Σ (y_i − ȳ)^2

## Sugestão de commit
```
docs: adiciona README e métricas/gráfico ao notebook de regressão linear
```

## Licença
MIT
