# Resolució

La resolució diu quants píxels caben en una polzada de la imatge: per a pantalla n'hi ha prou amb pocs, per imprimir en calen molts més.

## Què és la resolució

La **resolución** és el nombre de píxels que hi ha en una polzada (2,54 cm) de la imatge. S'escriu **ppp** (píxeles por pulgada), o **ppi** en anglès. A Photoshop sempre la veuràs com a píxeles/pulgada.

Hi ha dues dades que sovint es barregen, i convenen separar-les:

- **Dimensiones en píxels:** quants píxels té la imatge en total, per exemple 1080 × 1350. Diu quanta informació hi ha.
- **Resolución (ppp):** quants d'aquests píxels caben en una polzada de longitud. Diu com d'apretats estan, i per tant quina mida tindrà la imatge al paper.

Així, 300 ppp no vol dir «puc mostrar 300 píxels», sinó que **hi ha 300 píxels en cada polzada de longitud**. El nombre de píxels no canvia; el que canvia és quant espai ocupen.

### ppp o dpi?

En castellà, les dues sigles es tradueixen com a ppp, per això es confonen. Són dues coses diferents:

| | ppi (píxeles por pulgada) | dpi (puntos por pulgada) |
|---|---|---|
| Què mesura | La densitat de píxels d'una imatge digital | Els punts de tinta que una impressora pot posar en una polzada |
| De qui és | De la imatge (l'arxiu) | De la impressora (la màquina) |
| El fem servir a Photoshop | Sí, és el camp Resolución | No |

A classe, «dpi» i «ppp» se solen dir com a sinònims. El que ens importa quan editem és el **ppi**.

## Píxels i bitmap

Una imatge digital, com una foto, és un **bitmap** (mapa de bits): una graella de quadradets de color anomenats **píxels**. Cada píxel té un sol color, i de lluny, tots junts formen la imatge. Photoshop treballa sempre amb píxels quan edita imatges digitals.

Ho pots comprovar amb el zoom: obre una foto i amplia-la amb l'eina **Zoom** (Z) o amb **Ctrl + +**. A partir d'un cert punt deixes de veure una foto i veus els quadradets. A 100 % (**Ctrl + 1**), cada píxel de la imatge ocupa un píxel de la pantalla.

| | Bitmap (Photoshop) | Vectorial (Illustrator) |
|---|---|---|
| De què està feta | Una graella de píxels | Formes definides per fórmules matemàtiques |
| En ampliar | Es veuen els píxels i perd qualitat | Es veu igual de nítida |
| Quan es fa servir | Fotografies i retoc | Logotips i il·lustracions |

Per això la resolució importa a Photoshop i no a Illustrator: si una imatge té pocs píxels, no se'n poden inventar de bons.

## Relació entre píxels, ppp i mida impresa

Com que els píxels de la imatge no canvien, la resolució decideix quina mida tindrà quan s'imprimeixi:

> **mida impresa (polzades) = píxels ÷ ppp**

Per passar a centímetres, es multiplica per 2,54. Amb la mateixa imatge, **més ppp vol dir una mida impresa més petita**, perquè els píxels s'apleguen més.

| Imatge | A 72 ppp | A 300 ppp |
|---|---|---|
| 1080 × 1350 píxels (la peça de la sessió 1) | 38,1 × 47,6 cm | 9,1 × 11,4 cm |
| 6000 × 4000 píxels (foto de càmera) | 211,7 × 141,1 cm | 50,8 × 33,9 cm |

Si vols fer el càlcul a la inversa, per imprimir a una mida concreta a 300 ppp, necessites uns **2480 × 3508 píxels** per a un full A4.

## Quina resolució triar

**La resolució importa sobretot quan s'imprimeix.** La regla general és 72 ppp per a pantalla i 300 ppp per a impressió, però és una guia i no una regla absoluta ni única: depèn de l'ús, de la mida final i de la distància des d'on es mira.

| Per a què és | Resolución | Què cal tenir en compte |
|---|---|---|
| Pantalla, web i xarxes socials | 72 ppp | Qui mana són les **dimensions en píxels**. Una imatge de 1080 × 1350 es veu igual a 72 que a 300 ppp |
| Impressió de qualitat (fotos, revistes, cartells) | 300 ppp | És el valor habitual perquè l'ull no distingeixi els píxels en un paper |
| Impressora domèstica o mides grans | Al voltant de 150 ppp | Admet menys píxels, sobretot si es mira des de lluny |

Algunes idees importants:

- **72 ppp és una convenció**, no una regla de la pantalla: a l'ordinador, la resolución escrita en un fitxer no canvia com es veu. El que es veu són els píxels.
- **No s'ha d'ampliar una foto petita per imprimir-la.** Si l'amplies afegint píxels (amb Remuestrear activat), Photoshop crea píxels nous a partir dels que hi ha, i la imatge es veu més gran, però no més nítida.
- **El mode de color també canvia**: RGB per a pantalla, CMYK per a impressió (vegeu el Punt 1, menú Imagen > Modo).
- Com més píxels té una imatge, més pesa el fitxer.

## Comparació: 72 ppi i 300 ppi

| | 72 ppi | 300 ppi |
|---|---|---|
| Per a què s'usa | Pantalla, web i xarxes socials | Impressió de qualitat |
| Píxels en una polzada de longitud | 72 | 300 |
| Píxels en un centímetre | Uns 28 | Uns 118 |
| Píxels en un quadrat d'1 × 1 polzada | 5.184 | 90.000 |
| Mida impresa d'una imatge de 1080 × 1350 píxels | 38,1 × 47,6 cm | 9,1 × 11,4 cm |
| Com es veu en paper | Es distingeixen els píxels | Els píxels no es distingeixen a simple vista |
| Píxels necessaris per imprimir a la mateixa mida | Els que tingui la imatge | Uns 17 cops més que a 72 ppi |
| El valor de Resolución canvia com es veu a la pantalla? | No: el que importa són les dimensions en píxels | No: igual que a 72 ppi |

El 17 surt de dividir 300 per 72 i elevar-ho al quadrat: la mida es multiplica per 4,17 en cada direcció, i la superfície, per 17.

**Per resumir:** a la mateixa mida impresa, menys ppi vol dir menys informació (menys píxels) i més ppi vol dir més informació (més píxels). Un matís: el número de ppi per si sol no afegeix detall. La informació de la imatge és el nombre de píxels reals que té; el ppi només indica com s'apleguen quan s'imprimeix.

![72 ppi i 300 ppi en una polzada: menys i més píxels](svg/ppi.svg)

En una polzada, 72 ppi dona 72 píxels per costat i 300 ppi en dona 300: el mateix cercle es dibuixa amb molts més quadrets i la vora es veu més suau.

## On es canvia a Photoshop

Hi ha dos llocs:

- **Archivo > Nuevo:** quan crees el document, el camp **Resolución** fixa la resolució des del principi.
- **Imagen > Tamaño de la imagen** (Alt + Ctrl + I): per canviar la mida i la resolució d'una imatge que ja existeix.

A la finestra Tamaño de la imagen veuràs **Anchura**, **Altura** i **Resolución**, i una casella clau, **Remuestrear**. Es pot triar la unitat de cada mida (Píxeles, Pulgadas, Centímetros).

A dalt de la finestra també hi veus el **pes** de la imatge (a Tamaño de imagen, en MB) i les **Dimensiones** en píxels. Mira com canvia el pes quan actives Remuestrear i modifiques els píxels.

| Remuestrear | Què passa |
|---|---|
| **Desactivat** | Els píxels no canvien. Si canvies la Resolución, canvia la mida en cm (i al revés). És l'opció per preparar una imatge per imprimir sense tocar-la |
| **Activat** | Photoshop afegeix o treu píxels. Per reduir una imatge va bé; per ampliar-la, no millora la qualitat |

Per saber si una imatge t'ofereix prou resolució per imprimir: desactiva Remuestrear, posa 300 a Resolución i mira l'Anchura i l'Altura en centímetres. Si surt una mida igual o més gran que la que necessites, ho tens.

## Exemple: d'una imatge de pantalla a un cartell

En obrir una imatge, a Imagen > Tamaño de la imagen hi veus les **dimensiones en píxels**, l'Anchura i l'Altura (en la unitat que triis) i la **Resolución** en píxels/pulgada. Per imprimir-la en un cartell, no n'hi ha prou amb escriure 300 al camp Resolución:

| Què fas | Píxels | Mida impresa | Pes del fitxer |
|---|---|---|---|
| Imatge de 1080 × 1350 a 72 ppp (punt de partida) | 1080 × 1350 | 38,1 × 47,6 cm | El d'origen |
| Poses 300 ppp amb Remuestrear **desactivat** | No canvien | Es redueix a 9,1 × 11,4 cm | No canvia |
| Poses 300 ppp amb Remuestrear **activat**, mantenint els 38,1 × 47,6 cm | Passen a ser uns 4500 × 5600 | 38,1 × 47,6 cm | Augmenta molt |

La conclusió: la resolució no és un valor que es pugui «pujar» sense més. O bé es redueix la mida impresa, o bé Photoshop afegeix píxels inventats i la imatge no guanya detall. Per a un cartell de 40 × 50 cm a 300 ppp es necessiten uns **4724 × 5906 píxels reals**, i a 150 ppp, uns 2362 × 2953. Per això, abans d'imprimir, convé partir d'una foto original amb prou píxels, no d'una versió per a pantalla.

Atenció amb la paraula «mida»: pot voler dir la **mida impresa** (en cm) o el **pes del fitxer** (en MB). Canviar la resolució sense Remuestrear modifica la primera i deixa igual la segona.

## Remuestrear: per a què serveix i quines opcions té

**Remuestrear** (en anglès, *resample*) vol dir canviar el nombre de píxels d'una imatge: Photoshop n'afegeix o n'elimina. Quan no hi ha Remuestrear, només canvia la mida impresa. Quan hi és, es calcula una imatge nova amb més o menys píxels.

Com que els píxels nous s'han d'inventar a partir dels que ja existeixen, **Remuestrear no afegeix detall real**: el que fa és decidir de quina manera es calculen els píxels nous. Això ho tria el desplegable que apareix a la dreta de la casella Remuestrear, a Imagen > Tamaño de la imagen.

### Les opcions del desplegable

Els noms són els del desplegable de Photoshop en castellà. Les dreceres Opción + 1 a Opción + 8 (Alt + 1 a 8 a Windows) trien cada opció, en l'ordre de la llista.

| Opció | Per a què serveix | Exemple pràctic |
|---|---|---|
| **Automático** | Photoshop tria el mètode segons si ampliem o reduïm | Si no saps quina triar, deixa aquesta |
| **Conservar detalles 2.0** | Ampliar fotos conservant vores i detall. Té un control **Reducir ruido** | Una foto de 800 × 1000 píxels que vols passar a 1600 × 2000. Si veus gra, puja el valor de Reducir ruido |
| Conservar detalles (ampliación) | Versió anterior de l'opció anterior | La trobaràs en versions antigues o en tutorials antics |
| **Bicúbica más suavizada (ampliación)** | Ampliar amb transicions suaus i menys esglaons | Ampliar una mica una foto amb un cel amb degradats |
| **Bicúbica más enfocada (reducción)** | Reduir la mida mantenint la nitidesa | Una foto de càmera de 6000 × 4000 píxels que s'ha de pujar a una web a 1920 píxels d'ample |
| Bicúbica (degradados suaves) | Ús general, amb transicions suaus de to i un equilibri entre pes i qualitat | Una imatge amb molts degradats, com un cel de posta de sol |
| Por aproximación (bordes definidos) | Copia els píxels, sense barrejar-los. Manté les vores dures i el quadradet | Una icona de 16 × 16 píxels o una captura de pantalla que vols ampliar sense difuminar |
| Bilineal | Redimensionament senzill i ràpid, amb resultats menys precisos i més suaus | Gairebé no es fa servir; apareix perquè és un mètode clàssic |

### Cas pràctic: una imatge de baixa resolució per a una web

Primer cal saber **quina mena de «baixa resolució»** tens:

- **Pocs píxels** (per exemple, 600 × 400): és el problema real. A la web es veurà petita, o borrosa si l'ampliem.
- **Molts píxels amb 72 ppp:** no és cap problema per a una web. El valor de ppp no afecta com es veu a la pantalla.
- **Massa píxels** (per exemple, 6000 × 4000): tampoc és adequada per a la web, perquè pesa massa i la pàgina triga a carregar.

Amb Remuestrear, a cada cas:

1. **Pocs píxels i cal que es vegi més gran:** a Tamaño de la imagen, activa Remuestrear, tria **Píxeles** com a unitat, escriu l'Anchura que necessites i tria **Conservar detalles 2.0**. El resultat millora, però amb una ampliació gran no es recupera el detall que no hi era.
2. **Massa píxels:** Remuestrear activat, Píxeles, Anchura al valor que demani la web i **Bicúbica más enfocada (reducción)**. El fitxer pesa menys i la imatge continua nítida.
3. **Després:** exporta amb Archivo > Exportar > Exportar como (vegeu el Punt 1).

Si pots, **busca una versió original amb més píxels** abans d'ampliar. Ampliar amb Remuestrear és un recurs, no una solució màgica. A més, si vas ampliant i reduint la mateixa imatge una vegada i una altra, aniràs perdent qualitat: treballa sempre a partir de l'original.

## Fonts consultades

Elaborat amb informació d'aquestes pàgines, vistes als resultats de cerca (no obertes en complet):

- [Resolución, la frontera entre una imagen y una buena imagen (OCU)](https://www.ocu.org/tecnologia/camaras-digitales/noticias/resolucion-la-frontera-entre-una-imagen-y-una-buena-imagen): fórmula de la mida d'impressió.
- [Diferencia entre píxeles por pulgada y puntos por pulgada (Epson)](https://support.epson-europe.com/faqs/es/020020.pdf): ppi i dpi.
- [Tamaño de imagen, resolución y tamaño físico (UNLP)](https://perio.unlp.edu.ar/catedras/ecal/wp-content/uploads/sites/125/2022/04/Fotografia.-Tamano-de-imagen-resolucion-y-tamano-fisico.pdf): Remuestrear i mida física.
- [Resampling options in Photoshop (Adobe)](https://helpx.adobe.com/photoshop/desktop/crop-resize-transform/resize-adjust-resolution/resampling-options.html): llista d'opcions de Remuestrear i quan usar-les (vista als resultats de cerca).
