# Datensatz ESC Eurovision Song Contest #
Codebuch Stand 24.06.2025, aktualisiert 24.06.2025
erstellt von Gina Grad

## Inhalt
- edges_test_v2.csv (Edgelist)
- nodes_test_v2.csv (Nodelist)

## Ursprung und Datenerhebung
Die Daten stammen aus der offiziellen Webiste des ESC. Weitere bestimmungen zu dem Genre und den Ländern: 

Das Netzwerk ist ein *gerichtetes two-mode Akteursnetzwerk*.

**Umgang mit fehlgenden Werten**
Fehlende Werte werden nicht erfasst. Nicht "NA", stattdessen wird kein Wert eingetragen.

# EDGE-Attribute

**from**  
from	    ID des Knotens Land (bsp.: ger) -> Land gibt Punkte an, Land stimmt für

**to**
to 	       ID des Knotens Land (bsp.: ger) ODER ID des Knotens Genre -> Land bekommt Punkte, Genre bekommt Punkte

**weight**
weight	  Punkteverteilung der Jury des ESC (1 = 1 Punkt, 2 = 2 Punkte, [...] 12 = 12 Punkte)

**year***    
year  	2025 als Jahr

**neighbor**
neighbor  1 = Ja, es ist ein Nachbarland, 2 = Nein



# NODE-Attribute 
  
**id**  
id	    Abkürzung des Landes nach ISO (bsp.: ger), Abkürzung Genre ersten drei Buchstaben (bsp.: pop)
An dieser Stelle kommen alle verwendeten ISO-Abkürzungen
An dieser Stelle kommen alle verwendeten Genre-Abkürzungen

**name**
name	  Landname englisch, Genre-Titel (bsp.: Pop)
An dieser Stelle kommen alle verwendeten Genre-Titel

**region**
region	 1 - 7, Falls in bestimmter Region Zugehörigkeit zu anderen Ländern besteht (bsp.: 1)
1 = Northern Europe
2 = Central Europe
3 = Western Europe
4 = Southern Europe
5 = Southeastern Europe
6 = Eastern Europe
7 = Andere

**type**    
type  	1 als Land, 2 als Genre


##
