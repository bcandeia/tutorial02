# Planejamento de rotas de entrega — três abordagens

Este projeto resolve o mesmo problema de negócio — planejar rotas de entrega para
um Centro de Distribuição — de três formas diferentes, para comparar abordagens
e mostrar como a mesma pergunta pode ser respondida com ferramentas distintas.

**Objetivo:** mapear e otimizar as rotas de cinco entregadores partindo de um
Centro de Distribuição até 23 destinos, encerrando o turno em suas residências.

## Estrutura do projeto

```
tutorial02/
├── dados/
│   ├── destinos.csv         # endereços dos 23 destinos de entrega
│   └── residencias.csv      # endereços das residências dos entregadores
├── 1-arcgis-online-interface/
│   └── README.md            # tutorial passo a passo via interface (no-code)
├── 2-arcgis-api-python/
│   └── rotas_arcgis_api.py  # mesma análise, automatizada via ArcGIS API for Python
└── 3-open-source/
    └── rotas_geopandas_osmnx.py  # versão 100% open-source (geopandas + OSMnx)
```

## As três abordagens

### 1. Interface no-code (ArcGIS Online)
Tutorial passo a passo usando a interface do ArcGIS Online e a ferramenta
Network Analyst, sem escrever código. Ideal para quem precisa de uma solução
rápida sem depender de um time de desenvolvimento.

### 2. API Python do ArcGIS
A mesma análise, mas escrita como script usando a `arcgis` Python API — permite
automatizar, versionar e reexecutar a análise sem depender de cliques manuais,
mantendo o ecossistema Esri.

### 3. Stack open-source (GeoPandas + OSMnx)
Reprodução completa da análise usando apenas bibliotecas open-source, com dados
do OpenStreetMap. Não depende de licença paga — qualquer pessoa pode clonar este
repositório e rodar a análise localmente.

## Por que três versões?

Ferramentas diferentes fazem sentido em contextos diferentes: interface no-code
para prototipagem rápida, API proprietária quando a empresa já usa Esri em escala,
e stack open-source quando portabilidade e custo zero são prioridade. Este projeto
documenta as três, para que qualquer leitor possa escolher a abordagem mais
adequada ao seu contexto — ou comparar os resultados entre elas.
