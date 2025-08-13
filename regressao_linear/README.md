# 📊 Previsão de Vendas — Loja Fictícia (Agosto/2025)

> **Aviso:** Os dados usados neste projeto são **fictícios**, criados apenas para fins de **estudo** e **demonstração**. Não representam resultados reais da empresa.

## 🎯 Contexto do Problema
Queremos prever o total de vendas de **agosto/2025** antes do mês terminar, usando:
- Meses **fechados**: maio, junho e julho.
- **Parcial** de agosto (1º ao dia observado).

## 🧠 Metodologia
Quatro abordagens + faixa de cenários:
1. **Nowcast (ritmo atual)** — média diária observada em agosto × 31.
2. **Histórica (média 3m)** — mantém o realizado e usa a média dos 3 meses para os dias restantes.
3. **Tendência (regressão linear)** — tendência com maio–junho–julho para estimar agosto (mês 8).
4. **Combinada (60/40)** — 60% Nowcast + 40% Tendência.
5. **Faixa (baixo/alto)** — menor/maior média diária dos 3 meses aplicada aos dias restantes.

## 📂 Estrutura
- `historico_mensal_maio_junho_julho.csv` — histórico mensal (mês, dias_no_mes, total_vendas, media_diaria)
- `agosto_parcial_resumo.csv` — parcial de agosto (periodo, dias_observados, total_vendas_parcial, media_diaria_parcial)
- `notebook_previsao_vendas.ipynb` — notebook principal (Google Colab / Jupyter)
- Saídas geradas:
  - `vendas_maio_junho_julho.png`
  - `projecoes_agosto.png`
  - `resultados_projecao_agosto.csv`

## ▶️ Como executar
1. Abra o **Google Colab** e suba `historico_mensal_maio_junho_julho.csv` e `agosto_parcial_resumo.csv`.
2. Abra o `notebook_previsao_vendas.ipynb` e rode as células em ordem (todas têm comentários explicativos).
3. Para **atualizar diariamente**: edite `agosto_parcial_resumo.csv` (dias_observados e total_vendas_parcial) e rode novamente.

## 📜 Licença
MIT — uso livre para fins de estudo.
