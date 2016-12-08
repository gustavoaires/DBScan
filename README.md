# DBScan
Implementação do algoritmo de mineração de dados DBScan. Incluindo 3 medidas de similaridade: Euclidiana, Jaccard e Fading.

##Get started

1 - Baixe este projeto.

2 - Coloque o caminho do seu arquivo de entrada.
```python
    with open('tweets_30.tsv') as json_data:
```
3 - Escolha o formato do seu arquivo de entrada(JSON ou algum arquivo .txt dividido por algum caracter)
```python
    # A linha abaixo le um arquivo em formato JSON
    # points = json.load(json_data)
    
    # O codigo abaixo le um arquivo txt(tabulado)
    points = {}
    points['tweets'] = []
    for line in json_data:
        data = line.split('\t')
```
4 - Configure os parâmetros do algoritmo (eps e minPts)
```python
    # A funcao DBSCAN recebe um array de pontos, eps e minPoints.
    dbScan(points['tweets'], 0.3, 500)
```
5 - Coloque o caminho do seu arquivo de saída.
```python
    # Caminho do arquivo de saida dos clusters
    output_file = open('/Users/CAMINHO/DO/SEU/ARQUIVO/file.txt','a')
```
6 - Salve as edições.

7 - Abra o console e execute "python DBSCAN.py" 


## Observações

* O código está todo comentádo, a fim de facilitar a edição do mesmo.
