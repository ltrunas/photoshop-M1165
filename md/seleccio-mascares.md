# Selecció i màscares

Una **selecció** és una zona de la imatge on actuarà el que facis després (pintar, omplir, aplicar un ajust, esborrar). Una **màscara** és una manera de **amagar parts d'una capa sense esborrar-les**, i per això és **no destructiva**.

## <img class="ic" src="svg/ic-compass.svg" alt=""> El menú Selección

Els noms són els del menú de Photoshop en castellà.

| Ordre | Què fa | Drecera Windows | Drecera Mac |
|---|---|---|---|
| **Todo** | Selecciona tot el document | Ctrl + A | Cmd + A |
| **Deseleccionar** | Treu la selecció | Ctrl + D | Cmd + D |
| **Volver a seleccionar** | Recupera l'última selecció | Ctrl + Maj + D | Cmd + Maj + D |
| **Invertir** | Selecciona el que no estava seleccionat | Ctrl + Maj + I | Cmd + Maj + I |
| **Sujeto** | Selecciona la persona o l'objecte principal | — | — |
| **Cielo** | Selecciona el cel | — | — |
| **Rango de color…** | Selecciona per color | — | — |
| **Seleccionar y aplicar máscara…** | Millora les vores d'una selecció | Ctrl + Alt + R | Cmd + Opción + R |
| **Modificar** | Canvia la selecció (vegeu més avall) | — | — |
| **Guardar selección…** / **Cargar selección…** | Desa i recupera una selecció | — | — |

![Menú Selección de Photoshop](img/menu-seleccion.png)

## <img class="ic" src="svg/ic-cursor.svg" alt=""> Les eines de selecció

| Eina | Drecera | Per a què serveix |
|---|---|---|
| **Marco** | M | Selecció rectangular o el·líptica |
| **Lazo** | L | Selecció a mà alçada, o per punts amb el Lazo poligonal |
| **Selección de objetos** | W | Seleccionar un objecte o una persona de manera ràpida |

**Trucs amb el Marco:** **Maj** per fer un quadrat o un cercle perfecte, i **Alt** (**Opción** a Mac) per dibuixar des del centre.

### Sumar, restar i intersecar

![Les quatre maneres de combinar seleccions: Nueva selección, Añadir, Restar i Intersección](svg/seleccio-modes.svg)

A la barra de **opciones** hi ha quatre botons que controlen com es combina una selecció nova amb l'anterior:

- **Nueva selección:** substitueix l'anterior.
- **Añadir a la selección:** suma. Es pot fer amb **Maj** premut.
- **Restar de la selección:** treu. Es pot fer amb **Alt** (**Opción**) premut.
- **Intersección:** es queda només la part comuna.

## <img class="ic" src="svg/ic-scissors.svg" alt=""> Retocar una selecció

Amb una selecció activa, **Selección > Modificar** permet:

- **Ampliar** o **Reducir** la selecció uns píxels.
- **Suavizar** les vores.
- **Calar** (*feather*): difumina la vora perquè la transició no sigui dura. És important perquè una vora massa dura sembla retallada.

## <img class="ic" src="svg/ic-mask.svg" alt=""> Què és una màscara de capa

Una **màscara de capa** és una imatge en **blanc, negre i grisos** enganxada a una capa. Fixa't en aquest dibuix i en la regla de sota, que és tot el que cal recordar:

![Una capa més una màscara dona el resultat: el que és blanc es veu i el que és negre s'amaga](svg/mascara-regla.svg)


| Color a la màscara | Què passa a la capa |
|---|---|
| **Blanc** | Es **veu** |
| **Negre** | Està **amagat** |
| **Gris** | Es veu **a mitges** (transparència parcial) |

**Per què és millor que esborrar?** Perquè no es perd cap píxel. Si t'equivoques, pintes de blanc i el que s'havia amagat torna a aparèixer. És el mateix concepte que el retall no destructiu: es pot **rectificar**.


### <img class="ic" src="svg/ic-search.svg" alt=""> Què és l'alpha (α)

**Alpha** (o **canal alfa**) és la **informació de transparència** d'una imatge. En lloc de guardar-la com un color, Photoshop la guarda com una **imatge en escala de grisos** (*grayscale*): un únic canal amb tons que van del **negre al blanc**.

| <img class="ic" src="svg/ic-palette.svg" alt=""> To | <img class="ic" src="svg/ic-eye.svg" alt=""> Què vol dir | <img class="ic" src="svg/ic-hash.svg" alt=""> Valor |
|---|---|---|
| <img class="ic" src="svg/ic-dot-black.svg" alt=""> **Negre** | Transparent: **amagat** | 0 % |
| <img class="ic" src="svg/ic-dot-gray.svg" alt=""> **Gris** | **Mig transparent**: es veu a mitges | entre 0 i 100 % |
| <img class="ic" src="svg/ic-dot-white.svg" alt=""> **Blanc** | Opac: **es veu del tot** | 100 % |

![L'alpha com a escala de grisos: de negre (amagat) a blanc (es veu), passant pel gris](svg/alpha-grayscale.svg)

Una **màscara de capa** **és** això mateix: un canal alpha enganxat a la capa. Quan veus la màscara en blanc i negre, estàs veient la **transparència** de la capa **representada amb grisos**.

<img class="ic" src="svg/ic-bulb.svg" alt=""> **On el veig?** Obre **Ventana > Canales**. Quan guardes una selecció (**Selección > Guardar selección…**), Photoshop la desa com a canal alpha. També el pots veure amb **Alt** (**Opción** a Mac) + clic a la miniatura de la màscara.

### <img class="ic" src="svg/ic-wrench.svg" alt=""> Com es crea

1. Selecciona la capa al panell **Capas**.
2. Fes una selecció de la part que vols **mantenir** (per exemple, amb **Selección de objetos** o **Sujeto**).
3. Clica el botó de **màscara** de baix del panell **Capas** (el rectangle amb un cercle). La part seleccionada es veu i la resta s'amaga.

També pots fer-ho amb **Capa > Máscara de capa**, que ofereix opcions com *Mostrar todo* i *Ocultar todo*.

### <img class="ic" src="svg/ic-brush.svg" alt=""> Retocar la màscara amb el pincel

1. Clica la **miniatura de la màscara** (apareix un marc al voltant). **Si no, pintaràs sobre la imatge!**
2. Tria el **Pincel** (**B**).
3. Pinta de **negre** per **amagar** i de **blanc** per **tornar a mostrar**.
4. Prem **X**: **intercanvia** el negre i el blanc. Així **saltes d'un extrem a l'altre de l'escala de grisos** sense anar a la paleta de colors. Pinta, prem X i corregeix, i així tantes vegades com calgui.
5. Prem **D** per tornar als colors **per defecte** (negre i blanc).

![La tecla X intercanvia negre i blanc; la tecla D torna als colors per defecte](svg/pincel-x.svg)

<img class="ic" src="svg/ic-fog.svg" alt=""> **Per als grisos:** si vols una transició suau o una transparència a mitges, pinta amb un **pincel de vora suau** (poca **Dureza**) o baixa l'**Opacidad** del pincel a la barra de opciones. Així la màscara guarda tons de gris i la capa es veu a mitges.

### <img class="ic" src="svg/ic-gear.svg" alt=""> Altres operacions

| Què vols fer | Com |
|---|---|
| Veure només la màscara | **Alt** (**Opción**) + clic a la miniatura |
| Desactivar la màscara temporalment | **Maj** + clic a la miniatura |
| Moure la imatge sense moure la màscara | Clica la **cadena** entre la capa i la màscara per desvincular-les |
| Aplicar l'efecte a tot el document | Prova una **capa d'ajust**, que porta màscara |

## <img class="ic" src="svg/ic-bag.svg" alt=""> Per a què serveix? Un exemple real

Mira aquestes quatre imatges d'una botiga online. Sembla que hi hagi **quatre fotografies diferents**, però és **la mateixa foto del producte**: només han canviat **el color de les ratlles** i **el cel del fons**.

![Mateixa sabatilla, quatre variants: ratlles fúcsia, platejades, vermelles i negres, amb cels diferents](img/exemple-zalando-variants.png)

*Imatges d'exemple de Zalando.com (© Zalando / Adidas), reproduïdes només amb finalitat educativa.*

Com ho podrien haver fet amb Photoshop?

| Què canvia | Eina |
|---|---|
| Les **ratlles** de la sabatilla | **Selección** de les ratlles + capa d'ajust **Tono/Saturación** amb màscara |
| El **cel** del fons | **Selección > Cielo** + màscara de capa |
| Provar variants **sense perdre l'original** | Màscares i capes d'ajust (no destructiu) |

Així no cal tornar a fer la sessió de fotos per cada color. **Això és el que practicarem a la pràctica dels productes.**

## <img class="ic" src="svg/ic-pin.svg" alt=""> Per recordar

- Una **selecció** limita on actua el que fas.
- Una **màscara** amaga sense esborrar: **blanc = es veu, negre = amagat**.
- Si dubtes, **màscara abans que esborrar**.
- **Alpha** = la transparència en **escala de grisos**: negre 0 %, gris a mitges, blanc 100 %.
- Amb el **Pincel** sobre la màscara, **X** intercanvia negre i blanc i **D** torna als colors per defecte.
