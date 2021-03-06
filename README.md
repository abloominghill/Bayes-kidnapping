# Secuestro del Golden Retriver馃悤

<img width="290" align="right" src="https://i.pinimg.com/564x/95/35/62/953562d86b263fbf41119ae3b8c90e3d.jpg" />


Alguien a secuestrado a Bayes, el Golden Retriever ganador de premios de DataCamp. 

El secuestrador ha dejado pistas que podemos analizar: una nota de rescate, la versi贸n de un testigo y una huella a en la escena del crimen. 

A lo largo de la investigaci贸n se ir谩n recolectando m谩s datos para realizar an谩lisis que nos permitan ir reduciendo la lista de sospechosos.

Usaremos t茅cnicas como an谩lisis qu铆mico y frecuencia de letras para elegir al sospechoso correcto.

Este misterio se resolvi贸 a los largo del curso **"Introduction to Data Science in Python"**.

[Ver notebook](https://github.com/abloominghill/Bayes-kidnapping/blob/c01b3bcfa719ffd22367eb076255761107e15708/archivos/Introduction%20to%20Data%20Science%20in%20Python.ipynb)

---

### 馃攳 Informe del caso

- La primer pista que se ten铆a era una nota de rescate que se encontr贸 en la escena, se construy贸 una dataframe 'ransom.csv' que conten铆a la frecuencia con que aparec铆a las letras de la A a la Z en la nota.
- Una segunda pista fue un testig贸 que vi贸 una camioneta verde en la escena del crimen, pero s贸lo vi贸 las tres primeras letras, por lo que se contruy贸 una variable donde las cuatro letras faltantes se ingresaron como asterisco(*) para ingresarla en el sistema de b煤squeda de placas. Con esto se logr贸 tener una lista de cuatro sospechosos:
  - Fred Frequentist
  - Ronald Aylmer Fisher
  - Gertrude cox
  - kirstine smith
- Se obtuvo los registros de las tarjetad de cr茅dito de estos cuatro sospechosos para saber si alguno hab铆a hecho compras sospechosas. Se filtr贸 por aquellos que hubiesen hecho compras en Pet Paradise. Con esto reducimos la lista a dos sospechosos.
  - Fred frecuentista
  - Gertrude cox
- Se us贸 un diagrama de l铆neas para comparar la frecuencia de las letras en la nota de rescate con muestras de los dos principales sospechosos. Se descubri贸 que el secuestrador era Fred Frequentist. Ahora deb铆a encontrarse el lugar donde lo escond铆a.
- Los de la comisar铆a adquirieron datos de tel茅fonos m贸viles, que daban algunas de las ubicaciones de Fred en las 煤ltimas tres semanas. Las ubicaciones se dan como un conjunto de coordenadas x e y en un mapa. Para visualizar estas coordenadas, usamos un diagrama de dispersi贸n.
- Ten铆amos entonces tres posibles lugares: 
  - Blue Meadows Park
  - Shady Groves Campsite
  - Happy Mountain Trailhead
- Una huella de zapato en la escena del crimen conten铆a un tipo espec铆fico de grava. Seg煤n la distribuci贸n de los radios de grava, pod铆amos determinar d贸nde estuvo recientemente el secuestrador. Obtuvimos la distribuci贸n de los radios de grava de los tres lugares. Realizamos un gr谩fico de barras con la muestra recogida en la escena y por el comportamiento, se determin贸 que la arena proven铆a del campamento Shay Groves.
