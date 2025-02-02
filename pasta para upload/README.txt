Para utilizar o modelo

1. abra "EDA + Modelo de Previsao de Preco" em um jupyter notebook
2. crie uma célula e digite:

with open('modelo_1A.pkl', 'rb') as file:
    modelo_para_prev = pickle.load(file)

3. passe um dataframe ou dicionário com as seguintes features (os valores abaixo são exemplos)

{'id': 2595,
 'nome': 'Skylit Midtown Castle',
 'host_id': 2845,
 'host_name': 'Jennifer',
 'bairro_group': 'Manhattan',
 'bairro': 'Midtown',
 'latitude': 40.75362,
 'longitude': -73.98377,
 'room_type': 'Entire home/apt',
 'minimo_noites': 1,
 'numero_de_reviews': 45,
 'ultima_review': '2019-05-21',
 'reviews_por_mes': 0.38,
 'calculado_host_listings_count': 2,
 'disponibilidade_365': 355}

4. use a função modelo_para_prev(data) e pase seu dataframe ou dicionário no local "data" 