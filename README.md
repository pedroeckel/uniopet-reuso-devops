# Centralizador de códigos - Reuso de software com APIs

Este repositório centraliza os exemplos utilizados nas aulas de reuso de software da UniOpet. Os materiais estão organizados por aula para facilitar o acesso dos estudantes.

## Estrutura

- `aula-3/`: notebooks e imagens das aulas anteriores.
- `aula-4/`: pasta reservada para novos materiais.

## Requisitos

- Python 3.10+
- [Jupyter Notebook](https://jupyter.org/)
- Bibliotecas: `requests`, `folium`, `polyline`

Instale as dependências executando:

```bash
pip install jupyter requests folium polyline
```

## Como executar

1. Clone o repositório e acesse a pasta do projeto.
2. Inicie o Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Abra um dos arquivos `.ipynb` na pasta desejada e execute as células sequencialmente.

## Conteúdo da Aula 3

### 1-weather.ipynb
Consulta o clima atual de uma cidade utilizando a API do [OpenWeatherMap](https://openweathermap.org/).

### 2-route.ipynb
Integra as APIs do [OpenWeatherMap](https://openweathermap.org/) e do [OpenRouteService](https://openrouteservice.org/) para obter o clima e traçar uma rota entre duas cidades, exibindo o caminho em um mapa interativo com `folium`.

### 3-crud.ipynb
Demonstra operações de criação, leitura, atualização e exclusão em uma API REST pública (`api-ufpr.vercel.app`) reutilizando funções da biblioteca `requests`.

## Objetivo

Os exemplos visam ilustrar conceitos de **reuso de software**, mostrando como bibliotecas e APIs existentes podem ser combinadas para criar novas funcionalidades com pouco código.

