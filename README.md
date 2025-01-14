# Análise da Logística Loggi

Este projeto utiliza um notebook Jupyter para analisar dados logísticos da Loggi. O objetivo é realizar manipulação de dados, geolocalização e visualizações gráficas, proporcionando insights sobre entregas e hubs logísticos.

---

## Conteúdo do Projeto

### Principais Funcionalidades:

1. **Coleta de Dados**: Importação de dados logísticos de fontes públicas.
2. **Manipulação de Dados**: Estruturação e tratamento de dados em dataframes.
3. **Geolocalização**: Uso da API do Nominatim para obter coordenadas de hubs e entregas.
4. **Visualização**:
   - Mapas geográficos das entregas e hubs por região.
   - Gráficos estatísticos detalhados.

---

## Estrutura do Repositório

- `README.md`: Documentação do projeto.
`Projeto_de_estudo_Análise_da_logística_da_empresa_Loggi.ipynb`: Notebook com o código e análises.
- `deliveries.json`: Dados de entregas.
- `deliveries-geodata.csv`: Geolocalização de hubs e entregas.
- `distrito-federao.zip`: Conjunto dos dados para mapeamento.
- `requirements.txt`: Bibliotecas necessárias para o funcionamento do projeto.

## Baixando os Dados

Para baixar os dados usados no projeto, execute o código abaixo:
```bash
wget -q "https://raw.githubusercontent.com/andre-marcos-perez/ebac-course-utils/main/dataset/deliveries.json" -O dados/deliveries.json
wget -q "https://raw.githubusercontent.com/andre-marcos-perez/ebac-course-utils/main/dataset/deliveries-geodata.csv" -O dados/deliveries-geodata.csv
wget -q "https://geoftp.ibge.gov.br/cartas_e_mapas/bases_cartograficas_continuas/bc100/go_df/versao2016/shapefile/bc100_go_df_shp.zip" -O dados/distrito-federal.zip
```

Nota: os comandos para download dos dados já estão no notebook. Baixe os arquivos separadamente apenas se achar necessário. 

---

## Dependências

O projeto utiliza as seguintes bibliotecas:

- `pandas==1.5.3`
- `geopandas==0.13.2`
- `matplotlib==3.7.1`
- `seaborn==0.12.2`
- `geopy==2.3.1`
- `numpy==1.24.3`

Para instalar todas as dependências, execute:

```bash
pip install -r requirements.txt
