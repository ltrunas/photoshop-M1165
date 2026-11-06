# Retalls bàsics d'una imatge

**Retallar** vol dir **eliminar les parts de la imatge que no vols** per **reenfocar la composició**: canviar l'enquadrament, treure elements que sobren o adaptar la imatge a un format. A Photoshop es fa amb l'eina **Recortar**.

![L'eina Recortar i el seu marc](svg/retall.svg)

> **Abans de retallar, duplica la capa de fons** (**Ctrl + J**, **Cmd + J** a Mac). Així sempre pots tornar a la imatge original si en algun moment la vols recuperar. Retalla i treballa sobre la còpia.

## L'eina Recortar

- Es tria al panell d'eines (**Herramientas**), a la barra de l'esquerra: la icona té forma de **marc**. També amb la tecla **C**.
- L'eina ens deixa **escollir quina part de la imatge volem conservar**.
- Si no t'agrada el resultat, **Ctrl + Z** (Cmd + Z a Mac) per desfer.
- En activar-la apareix un **marc** a tot el voltant de la imatge. Arrossega les **nanses** (les cantonades i els costats) per decidir què conserves: el que queda a la zona fosca es retallarà.
- També pots **dibuixar un marc nou** arrossegant per la imatge, i **moure la imatge** dins del marc arrossegant-la.
- Per **confirmar** el retall: **Intro** (Enter), doble clic dins del marc o el botó de la marca de verificació a la barra d'opciones. Per **cancel·lar**: **Esc**.

### Dreceres mentre retalles

| Acció | Windows | Mac |
|---|---|---|
| Retallar des del centre | Alt + arrossegar una nansa | Opción + arrossegar una nansa |
| Mantenir o deixar anar la proporció | Maj + arrossegar una nansa | Maj + arrossegar una nansa |
| Girar el marc | Arrossegar fora del marc, a prop d'una cantonada | Igual |
| Canviar entre horitzontal i vertical | X | X |
| Confirmar / cancel·lar | Intro / Esc | Retorno / Esc |

## La barra de opciones de Recortar

Quan l'eina Recortar està activa, la barra de dalt mostra les opcions:

| Opció | Què fa |
|---|---|
| **Proporción** (desplegable) | Configura l'**aspect ratio** del marc, és a dir, quina forma té el retall. Veure la llista de sota. |
| **Enderezar** | Dibuixes una línia sobre quelcom que hauria de ser recte (un horitzó, una paret) i Photoshop gira la imatge perquè quedi a nivell. |
| **Superposición** (quadrícula) | Tria la guia visual del marc: regla de terços, quadrícula, diagonal… La **regla de terços** és la més útil per compondre. |
| **Borrar píxeles recortados** (casella) | Si està **marcada**, el que retalles s'esborra definitivament. Si està **desmarcada**, el retall és **no destructiu**: els píxels de fora es conserven amagats i, tornant a activar Recortar, pots recuperar-los i canviar el marc. |

### Els números i el botó d'intercanviar

Quan tries una proporció (a la captura, **5 : 7**), a la dreta apareixen dues caselles amb els números: l'**amplada** i l'**alçada**. Entre les dues hi ha el **botó de les dues fletxes**, que **intercanvia l'alçada per l'amplada**: serveix per passar el retall de **horitzontal a vertical** (o al revés) sense haver de tornar a triar la proporció. També ho fa la tecla **X**.

![Les caselles de proporció, el botó d'intercanviar, Borrar i Enderezar](img/recortar-intercanviar.png)

Al costat hi ha el botó **Borrar**, que buida les caselles perquè tornis a començar. No el confonguis amb la casella *Borrar píxeles recortados*: aquest botó només neteja els números. A la dreta, **Enderezar**, que ja hem vist.

### El desplegable Proporción

Aquí tries la forma del retall. Les opcions són:

![Desplegable Proporción de l'eina Recortar](img/recortar-proporcion.png)

| Opció | Què vol dir |
|---|---|
| **Proporción** (marcada per defecte) | Marc **lliure**: el dibuixes de la forma que vulguis. |
| **An. x Al. x Resolución** | Escrius l'ample, l'alt i la resolució: retalles a una **mida exacta**. |
| **Proporción original** | Manté la proporció de la imatge d'origen. |
| **1 : 1 (Cuadrado)** | Quadrat, com el de les xarxes socials. |
| **4 : 5 (8 : 10)**, **5 : 7**, **2 : 3 (4 : 6)** | Proporcions de **foto impresa**; 4:5 també s'usa a Instagram. |
| **16 : 9** | Format de pantalla, vídeo i presentacions. |
| **Dimensiones** (4 x 5 pulg. 300 ppp, 1024 x 768 px 92 ppp…) | Mides ja preparades, amb la seva resolució. Les de **pulgadas i 300 ppp** són per imprimir; les de **px** per pantalla. |
| **Nuevo ajuste preestablecido de recorte…** | Guarda una mida teva com a opció del menú. |
| **Eliminar el ajuste preestablecido de recorte…** | Esborra una opció guardada per tu. |

**Quina triar:** si ja saps on anirà la imatge (una foto impresa, una publicació quadrada, una pantalla), tria la proporció **abans** de retallar. Així no et sorprèn el format final.

> **Recomanació:** deixa **desmarcada** la casella de borrar píxeles recortados. Així pots reajustar el retall en qualsevol moment i no perds imatge.

## Retall no destructiu: reenquadrar després

Quan premem **Intro**, la imatge es **retalla**. Però aquesta eina és **no destructiva**: els canvis **no són definitius**. Photoshop guarda els píxels que han quedat fora del marc, només que no es veuen.

Per això, després de retallar, podem **reenquadrar**:

1. Tria l'eina **Mover** amb la tecla **V**.
2. Arrossega la imatge dins del llenç per **canviar l'enquadrament**: apareixen parts que havien quedat fora.
3. També pots tornar a l'eina **Recortar** (**C**) i el marc anterior reapareix perquè el canviïs.

**Important:** això només funciona si la casella **Borrar píxeles recortados** de la barra de opciones està **desmarcada**. Si està marcada, el que queda fora s'esborra de debò.

## Guardar el treball: normalment en PSD

Quan acabem, **guardarem normalment en PSD** (**Archivo > Guardar como**, **Ctrl + Maj + S**, **Cmd + Maj + S** a Mac). El PSD és el format propi de Photoshop i **conserva les capes**, la capa de fons duplicada, els retalls no destructius i tot el que has fet, així que pots reobrir-lo i seguir editant. Un JPG o un PNG no ho fa: només s'exporten al final, com a còpia per enviar o publicar.

## Altres maneres de retallar

- **Imagen > Recortar:** retalla la imatge a la **selecció** activa. Primer fes una selecció amb l'eina Marco (M) i després tria l'ordre. Si no hi ha cap selecció, l'ordre està en gris.
- **Imagen > Tamaño de lienzo** (**Alt + Ctrl + C**, **Opción + Cmd + C** a Mac): canvia la mida del llenç; si el redueixes, la imatge es retalla. També serveix per fer-lo **més gran** i afegir marge.
- **Imagen > Cortar…:** elimina automàticament les vores transparents o d'un color uniforme que envolten la imatge.

## Retallar o canviar la mida?

No són el mateix:

- **Retallar** treu una part de la imatge: la resta **conserva els mateixos píxels** i la mateixa qualitat.
- **Canviar la mida** (**Imagen > Tamaño de imagen**) fa tota la imatge més gran o més petita: canvia el nombre de píxels. Ho vam veure al punt de **Resolució**.

Moltes vegades les dues coses es combinen: primer **retalles** per l'enquadrament i després **ajustes la mida** per a la sortida final.

## Per recordar

- **Duplica la capa de fons** abans de començar, per poder tornar a l'original.
- L'eina Recortar és la **C**.
- Confirma amb **Intro**, cancel·la amb **Esc**.
- Tria la **Proporción** abans de retallar si ja saps el format final.
- Deixa desmarcat **Borrar píxeles recortados** per treballar sense perdre res.
- Després de retallar, amb **V** (Mover) pots **reenquadrar** la imatge.
- Guarda el treball en **PSD** per conservar les capes.
- **Enderezar** serveix per arreglar horitzons torts.
