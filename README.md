# Analise-de-Componentes-Principais
Após a criação do modelo de classificação para as posições da NBA, a ideia é utilizar técnicas para deixa-lo mais acertivo.

Então utilizando a analise de componentes principais, podemos melhorar a sua precisão. 

Primeiramente usamos o gráfico abaixo para analisar quantas componentes principais seria interessante usar.

![image](https://github.com/user-attachments/assets/e43d7399-5776-42be-a7f9-c8d74ae6490c)

É facil ver q após a terceira a variabilidade dos dados ja foi quase inteiramente explicada (99.2%)

Dado esse fato, após aplicar as C.P. vemos um gráfico de dispersão bem mais segmentado do que tinhamos anteriormente, vejao gráfico atual:

![grafico_dispersao](https://github.com/user-attachments/assets/49ac5dae-c4fb-481b-ac2e-708f15aa9f0e)

Utilizando ainda o metodo do KNN para modelar essa classifcação, chegamos nos seguintes resultados:

![image](https://github.com/user-attachments/assets/a113bbe6-a8d1-4b84-af5f-01675994c6be)

Observações:
- A precisão ( FP/FP+FN ) é mais alta para os C e PG, fato que eles possuem alturas e pesos bem diferentes, ficando facil deferencia-los dos demais.
- O suporte dos SF realmete deixa a desejar na amostra de teste ( na amostra de treino está dividida bem melhor).
- Consequência da última, a precisão e o recall quando se trata do SF estão bem distantes podendo indicar que o modelo está comentendo muito os Falsos Positivos.
- Apesar de 47.52% de acuracia, ja melhorou bastante em relação ao primeiro!
