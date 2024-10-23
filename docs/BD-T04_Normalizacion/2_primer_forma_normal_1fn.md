# 2. Primer Forma Normal (1FN)

 
<div style="background-color: #d6eaf8; color: black; padding: 5px;"> 
Una taula està en 1FN si i només si els valors que componen cada
atribut d'una tupla són atòmics. És a dir, en un atribut no han d'aparèixer
valors repetitius.</div>
---  


Per exemple, en la següent taula hi ha una sèrie de tipus de materials
existents en una ferreteria. Un material té un codi que l'identifica, la seua
descripció i les seues mides (la clau principal és el camp subratllat)

**MATERIALS**

_**COD-MAT**_ |  **DESCRIPCIÓ** |  **MIDES**  
---|---|---  
039  |  Cargol  |  3,5 - 5 - 7 - 9   
067  |  Arandella  |  2 - 5   
461  |  Broca  |  2,5 - 3 - 3,5   
  
Els problemes que planteja són els següents:

  * La falta de espai en el camp per als valors que puguen aparèixer o, pel contrari el desaprofitament de l'atribut quan existeixen pocs valors. 

  * La dificultat del tractament per a actualitzacions, consultes i recerques d'un valor determinat. 

  

**<u>Posar en 1FN</u>**

Per a passar a 1FN una taula que no ho estava **es descompon** en **dues**
distintes:

**A)** La **primera taula** serà la projecció de la taula original sobre els
següents atributs:

  * La clau de la taula original. 
  * Els atributs atòmics (els que contenen valors únics). 
  
**MATERIALS**

**COD-MAT** |  **DESCRIPCIÓ**  
---|---  
039  |  Cargol   
067  |  Arandella   
461  |  Broca


  
**B)** La **segona taula** serà la projecció de la taula original sobre els
següents atributs:

  * La clau de la taula original. 
  * Els atributs que tenen valors múltiples, distribuint aquestos valors múltiples en tuples distintes i per tant en una fila existirà un únic valor elemental. 

> La clau d'aquesta segona taula estarà formada per tots els atributs.

**MAT-MIDES**

**COD-MAT** | **MIDA**  
---|---  
039  |  3,5   
039  |  5   
039  |  7   
039  | 9   
067  |  2   
067  |  5   
461  |  2,5   
461  |  3   
461  |  3,5   
  

<u>**Nota**</u> 
<div style="background-color: #d6eaf8; color: black; padding: 5px;"> 
També haurem de ser capaços de detectar que no està en 1FN quan tenim uns
atributs multivaluats "encoberts". Per exemple, una variant de l'exemple
anterior podria ser:
</div>
<p></p>

**MATERIALS**

_**COD-MAT**_ |  **DESCRIPCIÓ** |  **MIDA1** | **MIDA2** |  **MIDA3** | **MIDA4**  
---|---|---|---|---|---  
039  |  Cargol  |  3,5  |  5 |  7 |  9  
067  |  Arandella  |  2  |  5 |  |   
461  |  Broca  |  2,5  |  3 |  3,5 |   
  


Es veu que es tracta d'una manera de "dissimular" els atributs multivaluats.
Estem davant del mateix cas que en l'exemple de dalt i tindrem els mateixos
problemes, i per tant la solució és la mateixa.  



Llicenciat sota la  [Llicència Creative Commons Reconeixement NoComercial
SenseObraDerivada 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/)

