# Informe de Laboratorio 3 - Ensamblaje de genomas y predicción de genes
Diego Hermosilla Alfaro

## Parte 1: El artículo genoma

Responde:

¿Cuántos genomas han sido depositados en GOLD? ¿Son los mismos de GENBANK?
  - Existen 11.598 organismos depositados en GOLD. Comparten muchos proyectos, pero en GENBANK se reportan una mayor cantidad de contribuciones.
  
¿Cuál es la distribución de procariontes y eucariontes secuenciados?
  - De procariontes se reportan 7.515 de bacterias y 256 arqueas, y de eucaritas se reportan 406 secuencias completadas.
  
¿Qué es el N50, L50, NG50?
  - Son referencias estadísticas que evaluan la calidad del ensamblaje de la secuencia. El N50 es la mínima cantidad de contigs que representan la mitad del genoma. El L50 es el número mínimo de contigs para alcanzar el N50. Y el NG50 es lo mismo que el N50, con la diferencia de que es el 50% del genoma conocido.
  
¿Cuál es el propósito de calcular estas estadísticas?
  - Estima la calidad del ensamblaje.
  
¿Cuál es el genoma que escogiste? Adjunta la referencia.
  - Escogí el genoma de *Orcinus orca*, también conocido como la orca. La referencia es: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4644735/
  
¿Cuál es el N50 del genoma que escogiste? ¿Y el NG50?
  - El N50 (contig) es de 70.300, y no se reporta el NG50.
  
¿Qué tipo de tecnología se uso para secuenciar el genoma que escogiste?
  - Toda la secuencia *shotgun* del genoma fue generada por la plataforma *Illumina HiSeq*.
  
¿Qué organismo escogiste, cuántos cromosomas tiene tu organismo y cuál es su tamaño?  
  - Escogí la ballena asesina, orca, *Orcinus orca*. Se reporta que tiene un cromosoma (genoma representativo) y tiene un largo de 2.372.919.875 pb. 
  
  
![imagen 1](https://raw.githubusercontent.com/dhermo/lab-3/master/globalstatistics.jpg)  
Imagen 1: Estadísticas globales del organismo *Orcinus orca*


## Parte 2: Predicción de genes

Responde:
¿Cuántos ORF o genes encontró ORFfinder?
  - ORFfinder encontró 7 ORFs
  
¿Cuántos ORF o genes encontró Glimmer?
  - Encontró 10 ORFs
  
¿Alguno de los genes predichos por estas herramientas coinciden?
  - Algunos ORFs coinciden en en alguno que otro codon stop, y en la dirección donde se encuentran codificados, pero ninguno coincide con los largos de los genes encontrados.
  
¿En qué hebra están codificados?
  - En ORFfinder se encontraron 3 en la hebra positiva y el resto en la negativa, mientras que en Glimmer 4 fueron encontradas en la hebra positiva y 6 en la negativa.
  
¿Qué tipo de programa es GLIMMER? ¿Ab initio o por homología?
  - Este programa trabaja por homología, utilizando datos interpolados para encontrar regiones codificantes a partir del modelo *Markov*
 
Describe los resultados encontrados con respecto a los genes que encontraste con GLIMMER y ORFfinder  
  - Luego de utilizar el blast, se encontró que todos los genes encontrados por ORFfinder y Glimmer tienen homologías con los genes de *Haemophilus influenzae*, siendo los genes predichos por Glimmer menos exactos que los de ORFfinder.  
