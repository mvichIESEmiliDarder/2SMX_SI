# PRÀCTICA D'UN ATAC DOS

**Objectiu:** Crear un bot que ataqui a un servidor web de forma que crei un atac de denegació de servei

## Material necessari
Emprarem per aquest atac els següents ordinadors:
 - 1 servidor Ubuntu amb un servidor Apache
 - 2 servidor Ubuntu per fer l'atac
 - 1 xarxa comuna

## Exercici 1
### Instruccions
Al servidor Ubuntu atacat, l'instal·larem un Apache i el mòdul d'status per tal de veure el nombre d'accessos
Al servidor Ubuntu atacant, crearem un script que faci 1000 atacs simultanis, que demanin 1000 vegades la pàgina del servidor

### Resultat
Hem de veure que el sevidor atacat, com que només ha de servir una pàgina molt simple, gaire bé no es veu afectat per l'atac de l'atacant

## Exercici 2
### Instruccions
Al servidor Ubuntu atacat, instal·larem un WordPress i el configurarem amb el mínim
Al servidor Ubuntu atacant, crearem un script que faci 1000 atacs simultanis, que demanin 1000 vegades la pàgina del servidor

### Resultat
En aquest cas, hem de veure que en servidor col·lapsa al cap de poc temps, ja que WordPress és molt més demandant i servir tantes pàgines fa que es denegui el servei 

## Exercici 3
### Instruccions
Deixarem el servidor Ubuntu atacat igual, però hem de crear una altra pàgina que controlarà l'atac. Mentre aquesta pàgina mostri 0, els atacants romandran pasius.
Però en el moment en que la pàgina mostri 1, els atacants han d'atacar sincronitzadament, el servidor de Wordpress

### Resultat
En aquest cas, hem de veure com el servidor col·lapsa molt més ràpidament després d'aquest DDOS o atac de denegació de servei distribuit
