# Projeto QSAR — CNN + Keras
**Disciplina:** Aprendizado Profundo | **Professor:** Rosalvo Neto

## Semente Aleatória Global: `42`
Fixada em NumPy, TensorFlow e Python random em todos os experimentos.

## Estrutura dos Notebooks

| Notebook | Dataset | class_0 | class_1 |
|---|---|---|---|
| `QSAR_BBBP.ipynb` | Blood-Brain Barrier Penetration | Não penetra BHE | Penetra BHE |
| `QSAR_BACE_C.ipynb` | BACE-1 Inhibition | Não inibidor | Inibidor BACE-1 |
| `QSAR_Toxicidade.ipynb` | Toxicidade | Não tóxico | Tóxico |

## Como usar

1. Coloque a pasta `Projeto2/` (com os três datasets) no mesmo diretório do notebook.
2. Ajuste `BASE_DIR` na célula "2. Caminhos do Dataset" se necessário.
3. Execute todas as células em ordem.

## Estrutura de cada Notebook (16 seções)

0. Instalação de dependências  
1. Imports e semente aleatória  
2. Definição de caminhos  
3. EDA — contagem e amostras visuais  
4. Hiperparâmetros globais  
5. Data Generators com augmentation  
6. Pesos de classe (desbalanceamento)  
7. Callback customizado de tempo  
8. **Modelo 1 — Baseline CNN** (4 blocos conv, do zero)  
9. **Modelo 2 — Fine-Tuning MobileNetV2** (2 estágios)  
10. Curvas de aprendizado  
11. Avaliação no teste (acc treino/val/teste + AUC-ROC)  
12. Matrizes de confusão + Curva ROC  
13. Discussão FP/FN  
14. Tabela de tempo de treinamento  
15. Tabela comparativa final (+ CSV)  
16. Análise comparativa e conclusões  

## Arquivos gerados por notebook

- `best_baseline_<dataset>.keras` — checkpoint do baseline  
- `best_finetune_<dataset>.keras` — checkpoint do fine-tuning  
- `samples_<dataset>.png` — amostras visuais  
- `curves_baseline_<dataset>.png` — curvas de aprendizado baseline  
- `curves_finetune_<dataset>.png` — curvas de aprendizado fine-tuning  
- `cm_<dataset>.png` — matrizes de confusão  
- `roc_<dataset>.png` — curvas ROC  
- `resultados_<dataset>.csv` — tabela comparativa exportada  
