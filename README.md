# Classificador de avaliações de delivery/e-commerce (PT-BR) com LoRA

Projeto de portfólio: classificação de sentimento e tema em avaliações em português,
comparando um baseline (TF-IDF + regressão logística), o modelo base (BERTimbau) e o
modelo ajustado com LoRA (PEFT), com publicação no Hugging Face.

> Status: 🚧 em construção (etapa 0 – setup concluído).

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

## Licença dos dados
A definir/confirmar na etapa 1 (dataset candidato: Olist, Kaggle).
