# Tech Challenge - Fase 3

Projeto da FIAP com foco em análise e previsão de atrasos de voos nos EUA.

## Arquivos

- `exploracao.ipynb`: EDA, limpeza e criação da base final.
- `supervisionado.ipynb`: classificação (`KNN`) e regressão (`RidgeCV`).
- `naoSupervisionado.ipynb`: clusterização com `MiniBatchKMeans`.
- `data/flights_limpas.csv`: dataset final usado nos modelos.

## Resumo do que foi feito

- Exploração dos dados com análise de atraso por companhia/aeroporto.
- Tratamento de dados e geração da variável alvo `BOL_DELAYED`.
- Modelagem supervisionada e não supervisionada, conforme pedido no desafio.

## Principais resultados

- **Classificação (KNN)**  
  Accuracy: `0.9425` | F1 (classe atraso): `0.88`
- **Regressão (RidgeCV)**  
  MAE: `4.3880` | RMSE: `5.9978` | R²: `0.6900`
- **Não supervisionado (MiniBatchKMeans)**  
  Accuracy: `0.7703` | F1 (classe atraso): `0.1872`

## Conclusão rápida

Os modelos supervisionados tiveram melhor desempenho para previsão de atraso.  
O não supervisionado ajudou na análise de padrões, mas com menor capacidade preditiva para voos atrasados.

## Como rodar

1. Instale as libs: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`.
2. Garanta os dados na pasta `data/`.
3. Execute os notebooks na ordem:
   - `exploracao.ipynb`
   - `supervisionado.ipynb`
   - `naoSupervisionado.ipynb`
