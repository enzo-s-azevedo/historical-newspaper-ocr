# Benchmark OCR para Jornais Históricos

Este repositório consiste em uma base de dados utilizada em um trabalho de pesquisa voltado à avaliação de técnicas de pré-processamento aplicadas em jornais antigos digitalizados para melhoria do desempenho de OCR.

A base contém as imagens originais, suas transcrições manuais (ground truth) e as versões preprocessadas utilizando diferentes configurações de pesos (thresholds) nas técnicas NLM (Non-Local Means) e TV (Total Variation).

O objetivo do trabalho associado a este repositório é analisar como essas variações de pré-processamento influenciam a Taxa de Erro de Caracteres (Character Error Rate - CER) na extração de texto com a ferramenta Dolphin-v2.

## Estrutura do Repositório

```text
dataset/
├── raw_images/        # Imagens originais digitalizadas
├── nlm/               # Imagens processadas com Non-Local Means
│   └── ...            # Diferentes pesos aplicados à técnica
└── tv/                # Imagens processadas com Total Variation
    └── ...            # Diferentes pesos aplicados à técnica
groundtruth/           # Transcrições manuais (.txt)
