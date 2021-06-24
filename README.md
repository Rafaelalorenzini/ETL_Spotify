# ETL Spotify

O projeto de ETL (extract, transform, load) foi proposto pela YouTuber Inglesa [Karolina Sowinska](https://www.youtube.com/channel/UCAxnMry1lETl47xQWABvH7g) e tem como objetivo passar mesmo que de forma básica pelos processos de ETL.

# Aquisição dos dados (Extrair)

Com uma conta do Spotify, é possível gerar um token que dará acesso às músicas que ouviu no tempo que escolher, para gerar basta ir no [site](https://developer.spotify.com/console/get-recently-played/). O token expira em pouco tempo, o ideal seria automatizar a atualização.

# Transformação
Após extrair os dados diretamente da API do Spotify no tempo que escolhi (uma semana), os dados são TRANSFORMADOS para uma arquivo JSON.  
Este é um bom caminho, pois posso escolher as informações que desejo colocar em um dicionário e depois transformar em um DataFrame do Pandas. 

#Carregamento
Utilizando o SQLAlchemy crio um banco de dados, esse banco de dados é então alimentado com os dados do DataFrame.


