# Amazon Deals Data Analysis

Este projeto realiza a coleta, tratamento, modelagem e análise de dados de ofertas da Amazon utilizando Python, pandas e matplotlib.

## Descrição

O objetivo deste projeto é consumir dados de ofertas em tempo real da Amazon através de uma API, estruturar esses dados em tabelas dimensionais e fato, realizar análises exploratórias e identificar os produtos com os maiores descontos. O projeto também inclui visualizações para facilitar a interpretação dos resultados.

## Etapas do Projeto

- **Coleta de Dados:**  
  Utilizei a API [Real-Time Amazon Data](https://rapidapi.com/real-time-amazon-data/api/real-time-amazon-data/) via RapidAPI para obter informações atualizadas sobre ofertas de produtos. Os dados foram salvos em formato JSON para facilitar o processamento.

- **Tratamento e Normalização:**  
  Os dados brutos em JSON foram carregados e normalizados em um DataFrame pandas, permitindo a manipulação tabular.

- **Modelagem Dimensional:**  
  Separei os dados em tabelas dimensão (`df_dim`) e fato (`df_fact`), seguindo boas práticas de modelagem de dados para análise.

- **Limpeza e Conversão de Dados:**  
  Realizei conversão de tipos (datas e valores numéricos), tratamento de valores ausentes e renomeação de colunas para facilitar a análise.

- **Análise Exploratória:**  
  Identifiquei os 5 produtos com maior desconto, calculei estatísticas básicas e explorei padrões nos dados.

- **Visualização:**  
  Criei gráficos de barras para comparar os maiores descontos com os demais produtos, utilizando matplotlib.

## Como rodar

1. Clone este repositório:
   ```sh
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```
2. Instale as dependências:
   ```sh
   pip install pandas matplotlib requests
   ```
3. Adicione sua chave de API no arquivo `headers.py` (veja o exemplo abaixo).
4. Execute o notebook `main.ipynb` para reproduzir as análises.

## Exemplo de `headers.py`

```python
key = "SUA_CHAVE_AQUI"
host = "real-time-amazon-data.p.rapidapi.com"
```

**Atenção:**  
Não compartilhe sua chave de API publicamente!

## Resultados

- Os 5 produtos com maior desconto foram destacados e visualizados em gráfico.
- O projeto serve como base para análises mais profundas, podendo ser expandido para outras categorias ou períodos.

## Possíveis Extensões

- Análise de tendências de preço ao longo do tempo.
- Comparação entre diferentes categorias de produtos.
- Automatização da coleta de dados para análises periódicas.

---

Sinta-se à vontade para contribuir ou sugerir melhorias!
