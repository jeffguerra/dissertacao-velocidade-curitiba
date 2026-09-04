# Velocidade e entorno urbano em Curitiba

Repositório de dados derivados e notebooks para reprodução das análises estatísticas da dissertação de Jefferson Artigas Guerra sobre velocidade operacional, velocidade insegura e ambiente construído em Curitiba.

## Conteúdo

- `data/base_h3_analitica.csv.gz`: base analítica agregada por célula H3 e hierarquia viária;
- `data/vizinhanca_rede.csv.gz`: relações de vizinhança da rede para 90 e 150 m;
- `notebooks/01_modelos_principais.ipynb`: descritivos, regressões lineares robustas, medida D e diagnósticos;
- `notebooks/02_robustez_espacial_e_figuras.ipynb`: MQO com erros agrupados, Moran global, SEM e figuras.

## Requisitos

Python 3.11 ou superior. Os principais pacotes utilizados são `pandas`, `numpy`, `statsmodels`, `scipy`, `matplotlib` e `h3`.

```bash
pip install -r requirements.txt
```

## Execução

Execute integralmente os notebooks nesta ordem:

1. `notebooks/01_modelos_principais.ipynb`
2. `notebooks/02_robustez_espacial_e_figuras.ipynb`

Os resultados são gravados automaticamente em `outputs/`.

## Dados restritos

A reprodução disponibilizada começa na base agregada H3–hierarquia. Os registros individuais do Estudo Naturalístico de Direção Brasileiro, incluindo telemetria por segundo, identificadores de condutores e viagens e vídeos, não são distribuídos por restrições de acesso e privacidade. O acesso a esses dados deve ser solicitado à instituição responsável pelo NDS-BR.

## Referência

Guerra, Jefferson Artigas. *Influence of the Urban Environment on Unsafe Speeds: An Approach Using Naturalistic Driving Data and H3 Indexing*. Universidade Federal do Paraná, 2026.
