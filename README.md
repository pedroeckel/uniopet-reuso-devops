# Repositório de Materiais - Reuso e DevOps

Este repositório centraliza os exemplos e atividades utilizados nas disciplinas ministradas pelo Prof. Pedro Eckel de Engenharia de Software da UniOpet. Os materiais agora estão organizados por disciplina (Reuso e DevOps) para facilitar o acesso dos estudantes.

## Estrutura

- `reuso/`: conteúdos da disciplina de reuso de software.
  - `aula-3/`: notebooks e imagens das aulas anteriores.
  - `aula-4/`: pasta reservada para novos materiais.
- `devops/`: conteúdos da disciplina de DevOps.

## Como clonar o repositório

Utilize o Git para clonar o repositório localmente:

```bash
# Via HTTPS
git clone https://github.com/<usuario>/api-python.git

# Via SSH
git clone git@github.com:<usuario>/api-python.git

cd api-python
```

## Requisitos

- Python 3.10+
- [Jupyter Notebook](https://jupyter.org/)
- Bibliotecas: `requests`, `folium`, `polyline`

Instale as dependências executando:

```bash
pip install jupyter requests folium polyline
```

## Como executar

1. Acesse a pasta do projeto.
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

