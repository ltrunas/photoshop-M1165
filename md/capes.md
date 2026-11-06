# Les capes

Les **capes** (*layers*) són el que fa que Photoshop sigui un programa tan potent. Podem imaginar-les com a **fulls de paper transparent apilats** els uns sobre els altres: cada full té una part de la imatge (una foto, un text, una forma, un color…) i, tots junts, formen la imatge final.

Això ens permet treballar sense risc: si retoquem, movem o esborrem una capa, les altres **no es modifiquen**. Per això, igual que a Illustrator, el panell de **Capas** és el més important de Photoshop: és on anirem treballant tota l'estona.

![Les capes són fulls transparents apilats](svg/capes-apilades.svg)

Amb les capes podem, per exemple:

- Posar un **text** sobre una fotografia i canviar-lo després sense tocar la foto.
- **Amagar** o mostrar parts de la imatge per comparar versions.
- Aplicar **ajustos de color** que es poden modificar o treure en qualsevol moment.
- Canviar l'**ordre**: el que està a dalt de tot del panell es veu per davant.

## El panell Capas

El panell **Capas** es troba normalment a **baix a la dreta** de l'espai de treball. Si no el veus, l'activem des del menú **Ventana > Capas** o amb la tecla **F7**.

Cada capa apareix com una fila amb la seva **miniatura** i el seu **nombre**. Una capa que està més amunt del panell es veu per davant de les que té a sota.

![Panell Capas amb Normal, Opacidad, Bloq., Relleno, l'ojo i la capa Fondo amb candau](img/panell-capas.png)

### Què hi ha a cada capa i a la part de dalt del panell

| Element | Què fa |
|---|---|
| **Ojo** (icona de l'ull) | Mostra o amaga la capa. Amagar no esborra: la capa continua al document. |
| **Miniatura** | Petit dibuix del contingut de la capa. |
| **Nombre** | Nom de la capa. Amb doble clic el podem canviar: posar noms clars ens estalvia molts maldecaps. |
| **Opacidad** | Com de transparent és la capa, de 0% (invisible) a 100% (opaca). |
| **Relleno** | Semblant a l'opacitat, però no afecta els efectes de la capa (per exemple, una ombra). |
| **Modo de fusión** | Tria com es barregen els colors de la capa amb els de sota (Multiplicar, Trama…). El menú desplegable és a dalt a l'esquerra del panell. |
| **Bloquear** | Candaus per protegir la capa: bloquejar els píxels transparents, la posició o tota la capa. |

### Els botons de baix del panell

A sota de la llista de capes hi ha una fila de botons per a les accions més usades. A la captura, d'esquerra a dreta:

![Panell Capas amb la fila de botons de baix: filtres, vincular, fx, màscara, ajust, grup, capa nova i paperera](img/panell-capas-botons.png)

| Botó | Què fa |
|---|---|
| **Primer botó** (pinzell amb un punt blau) | Accés ràpid a una funció nova d'aquesta versió. Deixa el cursor quiet a sobre per veure'n el nom exacte. |
| **Vincular capas** (cadena) | Uneix capes seleccionades per moure-les juntes. |
| **Añadir un estilo de capa** (*fx*) | Afegeix efectes com ombra, contorn o resplendor. |
| **Añadir máscara de capa** (rectangle amb cercle) | Crea una màscara per amagar parts d'una capa sense esborrar-les. |
| **Crear nueva capa de relleno o ajuste** (cercle mig ple) | Crea una capa de ajust de llum o color (la veurem més endavant). |
| **Crear un grupo nuevo** (carpeta) | Carpeta per ordenar diverses capes. |
| **Crear una capa nueva** (full amb un +) | Afegeix una capa en blanc. |
| **Eliminar capa** (paperera) | Esborra la capa seleccionada. També pots arrossegar-hi la capa. |

Si no recordes quin botó és quin, deixa el cursor quiet a sobre i Photoshop en mostra el nom.

### Modo de fusión i Opacidad

Són els dos controls de la fila de dalt del panell, i es poden canviar per a cada capa.

- **Modo de fusión** (el desplegable on posa *Normal*): decideix **com es barregen els colors** de la capa amb els de les capes de sota. En *Normal* la capa simplement tapa el que té a sota. Els modes més útils per començar:
  - **Multiplicar:** enfosqueix; el blanc desapareix. Va bé per a ombres.
  - **Trama:** aclareix; el negre desapareix. Va bé per a llums i resplendors.
  - **Superponer** i **Luz suave:** augmenten el contrast i el color de la capa de sota.
  - **Diferencia:** mostra la diferència entre dues capes.
  - **Color** i **Luminosidad:** apliquen només el color o només la llum de la capa.
- **Opacidad** (de 0% a 100%): com de **transparent** és la capa. Amb 100% es veu tota; amb 50% deixa veure el que hi ha a sota; amb 0% és invisible. Pots escriure el valor o arrossegar el petit control lliscant.
- **Relleno**: semblant a l'opacitat, però no afecta els efectes de la capa (per exemple, una ombra amb *fx* continua sent visible).

**Truc:** amb una eina de selecció o l'eina Mover activa, prem un número per canviar l'opacitat de la capa activa: **5** = 50%, **1** = 10%, **0** = 100%.

### Bloquejar una capa: el candau

A la fila **Bloq.** del panell hi ha unes icones petites que serveixen per **bloquejar atributs de la capa**, perquè no es puguin modificar per error:

| Icona | Què bloqueja |
|---|---|
| Quadrícula | Els **píxels transparents**: no es pot pintar a les zones buides. |
| Pinzell | Els **píxels de la imatge**: no es pot pintar ni retocar la capa. |
| Creu amb fletxes | La **posició**: la capa no es pot moure. |
| **Candau** | **Tot**: la capa queda completament protegida. |

Un exemple pràctic: si tens activada la **selección automática** amb l'eina **Mover**, en clicar a la imatge Photoshop agafa l'objecte i el pots moure sense voler. Si la capa té el **candau** (o la posició bloquejada), **no es pot moure**, i així no la desplaces per error.

Per això la capa **Fondo** surt amb un candau: Photoshop la protegeix per defecte. Per treure'l, clica al candau.

### Selecció automàtica de capes: Capa o Grupo

Quan tries l'eina **Mover** (**V**), a la barra d'opcions de dalt hi ha la casella **Selec. automática** i, al costat, un desplegable amb dues opcions:

![Desplegable de la Selec. automática amb les opcions Grupo i Capa](img/selec-automatica.png)

| Opció | Què passa quan cliques a la imatge |
|---|---|
| **Capa** | Photoshop selecciona la **capa individual** que hi ha sota el cursor. Si mous, només es mou aquella capa. |
| **Grupo** | Photoshop selecciona el **grup** sencer que conté aquella capa. Si mous, es mouen **totes les capes del grup** a la vegada. |

Així, amb **Capa** pots agafar un element concret, i amb **Grupo** mous diversos elements junts sense haver-los de seleccionar un per un. Per això és útil agrupar les capes (**Ctrl/Cmd + G**).

Si no vols que Photoshop triï la capa per tu, desactiva la casella **Selec. automática**: llavors el Mover només mou la capa que tinguis seleccionada al panell **Capas**. També pots mantenir premut **Ctrl** (**Cmd** a Mac) mentre cliques per triar la capa de manera temporal.

Recorda-ho amb el **candau**: una capa bloquejada no es mou, ni que la selecció automàtica la triï.

### El tauler d'escacs: què vol dir

Quan una capa té zones buides, a la imatge es veu un **tauler d'escacs** (quadres grisos i blancs). No forma part de la imatge: indica que aquella zona és **transparent**, és a dir, que no hi ha res. És el mateix que passa en un **PNG** amb fons transparent: el fons no és blanc, és transparent.

## Tipus de capes

No totes les capes són iguals. Les ens apareixen al panell amb una miniatura diferent segons el que contenen:

| Tipus | Com es reconeix | Per a què serveix |
|---|---|---|
| **Fondo** | Nom en cursiva i un **candau**. | És la capa original d'una foto quan l'obrim. Està bloquejada: per moure-la o fer-la transparent primer s'ha de desbloquejar (clic al candau). |
| **Capa normal** | Miniatura amb el contingut. | Una capa per pintar, enganxar imatges o retocar. |
| **Capa de texto** | Miniatura amb una **T**. | Conté un text que es pot editar en qualsevol moment. |
| **Capa de forma** | Miniatura amb una forma. | Conté una forma vectorial que es pot canviar de mida sense perdre qualitat. |
| **Objeto inteligente** | Icona petita a la miniatura. | Protegeix la imatge original: es pot canviar de mida o filtrar sense perdre qualitat. |
| **Capa de ajuste** | Miniatura amb la icona de l'ajust i una màscara al costat. | Aplica un ajust de color a les capes de sota sense tocar-les (ho veiem a l'apartat següent). |

Per a un primer curs, ens quedem sobretot amb les **capes normals**, el **Fondo**, el **texto** i les **capes de ajuste**.

## Capes d'ajust

Les **capes de ajuste** (*adjustment layers*) serveixen per canviar el color, la llum o el contrast d'una imatge **sense modificar els píxels originals**. L'ajust viu en una capa pròpia, a sobre de la foto, i afecta les capes que té a sota.

Això s'anomena treballar de manera **no destructiva**: en qualsevol moment podem amagar la capa d'ajust (amb l'**ojo**), canviar-ne els valors o esborrar-la, i la foto original continua intacta.

### Com es crea

- Amb el menú **Capa > Nueva capa de ajuste**.
- O amb el botó del panell **Capas** que diu **Crear nueva capa de relleno o ajuste** (el cercle partit en blanc i negre).

Trias l'ajust i s'obre el panell **Propiedades** amb els controls.

### Alguns ajustos habituals

| Ajust | Per a què serveix |
|---|---|
| **Brillo/Contraste** | Aclarir o enfosquir la imatge i donar-li més o menys contrast. |
| **Niveles** | Controlar millor les ombres, els mitjans tons i les llums. |
| **Curvas** | Control més fi del contrast i de la lluminositat. |
| **Tono/Saturación** | Canviar el color, la quantitat de color o la claredat. |
| **Equilibrio de color** | Afegir o treure un to de color (més càlid o més fred). |
| **Blanco y negro** | Passar la imatge a blanc i negre. |

Com que ens interessen sobretot el **retrat**, el **paisatge** i la **moda**, aquests ajustos seran els que farem servir més per donar to i ambient a les fotos.

### Capa d'ajust o menú Imagen > Ajustes?

També podem aplicar els mateixos ajustos des del menú **Imagen > Ajustes**, però això **canvia els píxels de manera permanent**. Per això, sempre que puguem, utilitzarem **capes de ajuste**.

## Operacions bàsiques amb capes

Aquestes són les accions que repetirem sempre. Quasi totes es troben al menú **Capa** i també al panell **Capas** (clic dret sobre una capa). A Mac, **Ctrl** és **Cmd**.

| Què vull fer | Com | Drecera (Windows) |
|---|---|---|
| **Crear** una capa nova | Botó **Crear una capa nueva** o **Capa > Nueva > Capa** | **Maj + Ctrl + N** |
| **Duplicar** una capa | Clic dret sobre la capa > Duplicar capa, o arrossegar-la al botó de nova capa o **Capa > Duplicar capa**. També: **Alt + arrossegar** amb Mover (**Opción** a Mac) | **Ctrl + J** |
| **Canviar el nom** | Doble clic sobre el nom | — |
| **Canviar l'ordre** | Arrossegar la capa amunt o avall al panell | — |
| **Seleccionar** diverses capes | Clic mantenint **Ctrl** (una a una) o **Maj** (un tram) | — |
| **Agrupar** capes | Seleccionar-les i **Capa > Agrupar capas** | **Ctrl + G** |
| **Fusionar** amb la de sota | **Capa > Combinar hacia abajo** | **Ctrl + E** |
| **Fusionar** diverses capes en una | Selecciona-les al panell i clic dret > **Combinar capas**, o **Capa > Combinar capas** | **Ctrl + E** (**Cmd + E** a Mac) |
| **Esborrar** una capa | Seleccionar-la i botó **Eliminar capa**, o tecla **Suprimir** | **Supr** |
| **Mostrar / amagar** | Clic a l'icona de l'**ojo** | — |

### Abans de treballar, comprova quina capa tens seleccionada

Les eines de Photoshop actuen **sempre sobre la capa seleccionada** (la que apareix marcada al panell). Si pintes, esborres o mous i no passa el que esperes, mira primer si tens triada la capa correcta.

### Consells

- **Duplica sempre la capa de fons** (Ctrl + J, Cmd + J a Mac) abans de començar a treballar. Així conserves l'original per si en algun moment vols tornar-hi, i treballes sobre la còpia.
- Posa **noms clars** a les capes («Fons», «Text», «Ajust de color»…) i agrupa-les per ordenar el document.
- Per **fusionar** diverses capes en una, selecciona-les al panell Capas (Ctrl/Cmd + clic) i usa el ratolí (clic dret > **Combinar capas**) o **Ctrl/Cmd + E**. Després ja no es poden separar.
- **Fusiona** o aplana les capes només al final, quan ja no hagis de fer més canvis: després no es poden separar.
- Treballa amb còpies i **capes de ajuste** per poder desfer qualsevol decisió.

## Exercici: composició amb capes duplicades

Per practicar tot això, farem una composició amb un fons i unes mans.

1. **Descarrega de Moodle** el contingut: la imatge del **fons** i les imatges de les **mans**.
2. Obre-les a Photoshop: cada imatge s'obre en un **lienzo** (document) diferent.
3. Fes la **composició** duplicant les capes: porta cada mà al document del fons i col·loca-la amb l'eina **Mover**.

![Composició de referència: tres mans sobre un fons, amb quatre documents oberts i les capes HAND 01, 02 i 03](img/exercici-composicio.png)

**Duplicar mentre mous (el més ràpid):** amb la capa seleccionada i l'eina **Mover** (**V**), mantén premuda **Alt** (**Opción** a Mac) i arrossega l'element: Photoshop **crea una còpia automàticament** i tu mous la còpia, deixant l'original al lloc. Cal tenir la capa seleccionada (o la *Selec. automática* activada) perquè mogui la capa correcta.

Per duplicar també pots fer servir **Ctrl/Cmd + J** (dins del mateix document) o **clic dret sobre la capa > Duplicar capa**. Aquesta segona opció obre una finestra que et pregunta el **destino** (el document on vols enviar la còpia), i serveix per passar una capa d'un lienzo a un altre quan en tens diversos oberts.

A la imatge de referència, el document del fons té les capes del fons i de les tres mans, cadascuna amb el seu nom: així pots ordenar-te i canviar-ne la posició sense tocar les altres.

## Per recordar

- El panell **Capas** (**F7**) és on treballem: cada capa és un full transparent apilat sobre els altres.
- Una capa que està més amunt es veu per davant de les de sota.
- L'**ojo** amaga una capa; **Opacidad** la fa més o menys transparent.
- Les eines actuen sobre la **capa seleccionada**.
- La capa **Fondo** està bloquejada: cal desbloquejar-la per moure-la.
- Les **capes de ajuste** canvien el color i la llum **sense modificar la foto original**.
- **Ctrl + J** duplica, **Ctrl + G** agrupa i **Ctrl + E** fusiona.
