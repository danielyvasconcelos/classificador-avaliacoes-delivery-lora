# Classificador de avaliações de delivery/e-commerce (PT-BR) com LoRA

Projeto de portfólio: classificação de sentimento e tema em avaliações em português,
comparando um baseline (TF-IDF + regressão logística), o modelo base (BERTimbau) e o
modelo ajustado com LoRA (PEFT), com publicação no Hugging Face.

> Status: 🚧 em construção (etapa 1 – exploração dos dados).

## Estrutura

```
data/raw/        dados originais (não versionados)
data/processed/  dados tratados e splits (não versionados)
notebooks/       exploração
src/             scripts: preparar dados, treinar, avaliar
models/          saídas de treino (não versionadas)
reports/         métricas, figuras, análise de erros
```

## Segredos
Nunca coloque tokens no código. Use os Segredos do Colab ou variáveis de ambiente
(veja `.env.example`).

## Dados
- **Fonte:** [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) (Kaggle), ~100 mil pedidos de 2016 a 2018.
- **Licença:** CC BY-NC-SA 4.0 (uso não comercial, com atribuição e compartilhamento pela mesma licença).
- **Como obter:** baixe o zip no Kaggle (requer login), extraia e coloque `olist_order_reviews_dataset.csv` em `data/raw/olist/`. Os dados não são versionados.
- **Observação:** nomes de empresas e parceiros nos textos foram substituídos por nomes de casas de *Game of Thrones* pelo provedor.
