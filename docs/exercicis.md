# Exercicis

![](icon_activity.gif)

## Exercici 1

Normalitzar la taula relacional que té com a graf de dependències funcionals
el següent:

![](T4_Ex_1.png)

Podeu normalitzar-ho tot directament, sense haver de passar primer per 2FN ,
3FN i FNBC.

![](icon_activity.gif)

## Exercici 2

En un Institut tenen distribuïda la informació en els següents fitxers:

**FGAL** CODAL  
NUMEX  
COGNOM1  
COGNOM2  
NOM  
CODCURS  
NOMCURS |  **FASSIGN** CODCURS   
CODASSIG  
NOMCURS  
NOMASSIG  
CODPROF  
NOMPROF |  **FPROF** CODPROF   
NOMPROF  
CODCURS1  
CODASSIG1  
CODCURS2  
CODASSIG2  
.  
.  
.  
CODCURS10  
CODASSIG10 |  **FCURS** CODCURS   
NOMCURS  
CODTUTOR  
NOMTUTOR  
CODASSIG1  
CODASSIG2  
.  
.  
.  
CODASSIG17  
---|---|---|---  
  
Normalitzeu els fitxers, si els considerem taules d’una Base de Dades. Heu de
parar especial atenció a veure si està en 1FN.

![](icon_activity.gif)

## Exercici 3

La factura d'un hotel és la següent:

| HOTEL PRIMAVERA |  |  | Factura: | 1934  
---|---|---|---|---  
Data: | 15 desembre 2009 |  |  |  |   
|  |  |  |  |   
Client: | Andreu Torlà Gomis |  |  | Habitació: | 202  
DNI: | 18.012.345-W |  |  | Tipus: | Doble  
Domicili: | C/ Palanques, 5 |  |  | Tarifa: | 2  
CP: | 12004 |  |  |  |   
Població: | Castelló |  |  |  |   
Telèfon: | 964-223344 |  |  |  |   
|  |  |  |  |   
Núm. pers.: | 2 |  |  |  |   
|  |  |  |  |   
Codi | Concepte | Quantitat | Preu unitari | Total |   
|  |  |  |  |   
2 | Estància Mitja Pensió | 3 | 65 | 195 |   
45 | Dinar | 2 | 15 | 30 |   
23 | Consum Bar | 1 | 5,3 | 5,3 |   
|  |  |  |  |   
|  |  |  |  |   
|  |  |  |  |   
| Base imponible: | 230,3 |  |  |   
| IVA (16%): | 36,85 |  |  |   
|  | \---------- |  |  |   
| Total : | 267,15 |  |  |   
  
Si considerem tota la informació en una única taula tindrem:

**FACTURA**

NUMFACT  
DATA  
NUMHAB  
TIPHAB  
TARHAB  
NOMCLI  
DNICLI  
ADRCLI  
CPCLI  
CIUCLI  
TELCLI  
NUMPERS | COD1   
CONCEPTE1  
QUANT1  
PREU1  
TOTAL1  
.  
.  
COD15  
CONCEPTE15  
QUANT15  
PREU15  
TOTAL15 | TOTAL   
IVA  
TOTALIVA  
TOTFAC  
---|---|---  
  
Intenteu normalitzar-la. Pareu especial atenció aveure si està en 1FN.



Llicenciat sota la  [Llicència Creative Commons Reconeixement NoComercial
SenseObraDerivada 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/)

