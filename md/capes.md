# Les capes

Les **capes** (*layers*) són el que fa que Photoshop sigui un programa tan potent. Podem imaginar-les com a **fulls de paper transparent apilats** els uns sobre els altres: cada full té una part de la imatge (una foto, un text, una forma, un color…) i, tots junts, formen la imatge final.

Això ens permet treballar sense risc: si retoquem, movem o esborrem una capa, les altres **no es modifiquen**. Per això, igual que a Illustrator, el panell de **Capas** és el més important de Photoshop: és on anirem treballant tota l'estona.

Amb les capes podem, per exemple:

- Posar un **text** sobre una fotografia i canviar-lo després sense tocar la foto.
- **Amagar** o mostrar parts de la imatge per comparar versions.
- Aplicar **ajustos de color** que es poden modificar o treure en qualsevol moment.
- Canviar l'**ordre**: el que està a dalt de tot del panell es veu per davant.

## El panell Capas

El panell **Capas** es troba normalment a **baix a la dreta** de l'espai de treball. Si no el veus, l'activem des del menú **Ventana > Capas** o amb la tecla **F7**.

Cada capa apareix com una fila amb la seva **miniatura** i el seu **nombre**. Una capa que està més amunt del panell es veu per davant de les que té a sota.

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

| Botó | Què fa |
|---|---|
| **Vincular capas** | Uneix capes seleccionades per moure-les juntes. |
| **Añadir un estilo de capa** (*fx*) | Afegeix efectes com ombra, contorn o resplendor. |
| **Añadir máscara de capa** | Crea una màscara per amagar parts d'una capa sense esborrar-les. |
| **Crear nueva capa de relleno o ajuste** | Crea una capa de ajust (la veurem més endavant). |
| **Crear un grupo nuevo** | Carpeta per ordenar diverses capes. |
| **Crear una capa nueva** | Afegeix una capa en blanc. |
| **Eliminar capa** | Esborra la capa seleccionada (la paperera). |

Si no recordes quin botó és quin, deixa el cursor quiet a sobre i Photoshop en mostra el nom.

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
| **Duplicar** una capa | Clic dret sobre la capa > Duplicar capa, o arrossegar-la al botó de nova capa o **Capa > Duplicar capa** | **Ctrl + J** |
| **Canviar el nom** | Doble clic sobre el nom | — |
| **Canviar l'ordre** | Arrossegar la capa amunt o avall al panell | — |
| **Seleccionar** diverses capes | Clic mantenint **Ctrl** (una a una) o **Maj** (un tram) | — |
| **Agrupar** capes | Seleccionar-les i **Capa > Agrupar capas** | **Ctrl + G** |
| **Fusionar** amb la de sota | **Capa > Combinar hacia abajo** | **Ctrl + E** |
| **Esborrar** una capa | Seleccionar-la i botó **Eliminar capa**, o tecla **Suprimir** | **Supr** |
| **Mostrar / amagar** | Clic a l'icona de l'**ojo** | — |

### Abans de treballar, comprova quina capa tens seleccionada

Les eines de Photoshop actuen **sempre sobre la capa seleccionada** (la que apareix marcada al panell). Si pintes, esborres o mous i no passa el que esperes, mira primer si tens triada la capa correcta.

### Consells

- Posa **noms clars** a les capes («Fons», «Text», «Ajust de color»…) i agrupa-les per ordenar el document.
- **Fusiona** o aplana les capes només al final, quan ja no hagis de fer més canvis: després no es poden separar.
- Treballa amb còpies i **capes de ajuste** per poder desfer qualsevol decisió.

## Per recordar

- El panell **Capas** (**F7**) és on treballem: cada capa és un full transparent apilat sobre els altres.
- Una capa que està més amunt es veu per davant de les de sota.
- L'**ojo** amaga una capa; **Opacidad** la fa més o menys transparent.
- Les eines actuen sobre la **capa seleccionada**.
- La capa **Fondo** està bloquejada: cal desbloquejar-la per moure-la.
- Les **capes de ajuste** canvien el color i la llum **sense modificar la foto original**.
- **Ctrl + J** duplica, **Ctrl + G** agrupa i **Ctrl + E** fusiona.
