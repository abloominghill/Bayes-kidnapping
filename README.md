# Secuestro del Golden Retriver🐕

<img width="290" align="right" src="https://i.pinimg.com/564x/95/35/62/953562d86b263fbf41119ae3b8c90e3d.jpg" />


Alguien a secuestrado a Bayes, el Golden Retriever ganador de premios de DataCamp. 

El secuestrador ha dejado pistas que podemos analizar: una nota de rescate, y la versión de un testigo que vió una camioneta en la escena del crimen. 

A lo largo de la investigación se irán recolectando más datos para realizar análisis que nos permitan ir reduciendo la lista de sospechosos.

Usaremos técnicas como análisis químico y frecuencia de letras para elegir al sospechoso correcto.

Este misterio se resolvió a los largo del curso **"Introduction to Data Science in Python"**.

[Ver notebook](https://github.com/abloominghill/Bayes-kidnapping/blob/ee7a3b01238b77ef64e7f4c064106bdee1340cb2/archivos/Introduction%20to%20Data%20Science%20in%20Python.ipynb)

---

### 🔍 Informe del caso

- La primer pista que se tenía era una nota de rescate que se encontró en la escena, se construyó una dataframe 'ransom.csv' que contenía la frecuencia con que aparecía las letras de la A a la Z en la nota.
- Una segunda pista fue un testigó que vió una camioneta verde en la escena del crimen, pero sólo vió las tres primeras letras, por lo que se contruyó una variable donde las cuatro letras faltantes se ingresaron como asterisco(*) para ingresarla en el sistema de búsqueda de placas. Con esto se logró tener una lista de cuatro sospechosos:
  - Fred Frequentist
  - Ronald Aylmer Fisher
  - Gertrude cox
  - kirstine smith
- Se obtuvo los registros de las tarjetad de crédito de estos cuatro sospechosos para saber si alguno había hecho compras sospechosas. Se filtró por aquellos que hubiesen hecho compras en Pet Paradise. Con esto reducimos la lista a dos sospechosos.
  - Fred frecuentista
  - Gertrude cox
- Se usó un diagrama de líneas para comparar la frecuencia de las letras en la nota de rescate con muestras de los dos principales sospechosos. Se descubrió que el secuestrador era Fred Frequentist. Ahora debía encontrarse el lugar donde lo escondía.
- Los de la comisaría adquirieron datos de teléfonos móviles, que daban algunas de las ubicaciones de Fred en las últimas tres semanas. Las ubicaciones se dan como un conjunto de coordenadas x e y en un mapa. Para visualizar estas coordenadas, usamos un diagrama de dispersión.
- Teníamos entonces tres posibles lugares: 
  - Blue Meadows Park
  - Shady Groves Campsite
  - Happy Mountain Trailhead
- Una huella de zapato en la escena del crimen contenía un tipo específico de grava. Según la distribución de los radios de grava, podíamos determinar dónde estuvo recientemente el secuestrador. Obtuvimos la distribución de los radios de grava de los tres lugares. Realizamos un gráfico de barras con la muestra recogida en la escena y por el comportamiento, se determinó que la arena provenía del campamento Shay Groves.
