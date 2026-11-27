# Canviar el color d'un producte

En una botiga online, el mateix producte surt en **molts colors**, però només s'ha fotografiat **una vegada**. Els altres colors es fan a Photoshop. Aquí ho fem amb **tres colors de marca**, definits per un **codi hexadecimal**.

![Mateixa sabatilla en tres colors: blau marí, verd bosc i mostassa](img/exemple-sabatilles-colors.jpg)

*Exemple orientatiu dels tres colors. El resultat de cada persona pot variar.*

## <img class="ic" src="svg/ic-hash.svg" alt=""> Què és un codi hexadecimal

Un color a pantalla es barreja amb **vermell, verd i blau** (RGB). El codi **#1F3A5F** són tres parelles de xifres: la primera és el **vermell**, la segona el **verd** i la tercera el **blau**.

| Color | Codi | RGB (vermell · verd · blau) | Nom de la capa |
|---|---|---|---|
| Blau marí | **#1F3A5F** | 31 · 58 · 95 | `color_blau` |
| Verd bosc | **#2F5D46** | 47 · 93 · 70 | `color_verd` |
| Mostassa | **#D4A017** | 212 · 160 · 23 | `color_mostassa` |

## <img class="ic" src="svg/ic-steps.svg" alt=""> Pas a pas

1. **Duplica la capa de fons** (**Ctrl + J** a Windows, **Cmd + J** a Mac). Mai treballis sobre l'original.
2. **Selecciona la sabatilla** (les dues) amb **Selección de objetos** (**W**) o **Selección > Rango de color…**. Afegeix zones amb **Maj**, resta amb **Alt** (**Opción** a Mac) i suavitza amb **Calar**.
3. Amb la selecció activa: **Capa > Nueva capa de relleno > Color sólido…**. Al **Selector de color**, escriu el codi al camp **#**. **La selecció es converteix en la màscara de la capa.**
4. Posa la capa en **Modo de fusión: Color**. Així el color nou es veu, però **es conserven els reflexos i les ombres** de la sabata.
5. Retoca la **màscara** amb el **Pincel** (**B**): **negre amaga, blanc mostra, X intercanvia**. Treu les aurèoles de color i les taques a les cames.
6. Dona un **nom** a la capa (per exemple `color_blau`): doble clic sobre el nom.
7. Repeteix els passos 3 a 6 amb els altres dos colors. Amaga amb l'**ull** els que no estiguis veient.

Així hauria de quedar la selecció del pas 2: les **formigues** segueixen la vora del cuir i **deixen fora** el fons, la pell, les soles i **els cordons**. Així el color nou només pinta el cuir i els cordons es queden crema.

![Selecció de la part vermella de les dues sabates, amb les soles, la pell i els cordons fora](img/seleccio-sabatilles.jpg)

## <img class="ic" src="svg/ic-brush.svg" alt=""> Dues maneres de canviar el color

Hi ha dues maneres de pintar de color una sabata. Totes dues fan servir una **capa d'ajust amb màscara**, però no donen el mateix resultat.

| | **Relleno de color sólido + Modo Color** | **Tono/Saturación + Colorear** |
|---|---|---|
| Com es crea | **Capa > Nueva capa de relleno > Color sólido…** | **Capa > Nueva capa de ajuste > Tono/Saturación…** i marcar **Colorear** |
| Com es tria el color | Amb el **codi hexadecimal** (camp **#**) | Amb els valors **Tono**, **Saturación** i **Luminosidad** |
| El **hex** | **Sí**: s'escriu directament. | **No té camp per al hex.** |
| Precisió | **Exacta** respecte al codi (afinant la llum). | **Aproximada**: només n'obtens un to semblant. |
| Quan va bé | Quan et donen **un codi de marca**. | Per provar un to **a ull**, ràpid. |

### I si vull fer servir Tono/Saturación amb un codi hex?

El quadre de **Colorear** **no té camp hex**. Per acostar-t'hi:

1. Obre el **Selector de color** (clic al color de primer pla) i escriu el codi al camp **#**.
2. Mira el valor **H** (to) que et mostra el Selector de color.
3. A **Tono/Saturación**, marca **Colorear** i posa aquest valor a **Tono** (de 0 a 360). A **Saturación** posa un valor de partida (vegeu la taula).
4. Ajusta **Saturación** i **Luminosidad** a ull fins que s'assembli. Comprova-ho amb el **Cuentagotas** (**I**).

Valors orientatius per començar (després s'ha d'afinar a ull):

| Color | Codi | **Tono** | **Saturación** (de partida) |
|---|---|---|---|
| Blau marí | #1F3A5F | 215 | 51 |
| Verd bosc | #2F5D46 | 150 | 33 |
| Mostassa | #D4A017 | 44 | 80 |

**No et sortirà exactament el codi**: el mode **Colorear** manté la llum de la foto i la saturació no funciona igual que al Selector de color. Si el que et demanen és **un codi concret**, fes servir **Color sólido + Modo Color**.

### I si em donen els valors de Tono, Saturación i Luminosidad?

Aleshores **Tono/Saturación amb Colorear** és la manera directa: **escriu els valors als tres camps**.

- **Tono:** de **0 a 360**. Es posa tal qual.
- **Saturación:** de **0 a 100**. Es posa tal qual.
- **Luminosidad:** va de **−100 a +100** i és un **ajust relatiu**: **no** és la lluminositat absoluta del color. Mou-la fins que el to quedi com vols i comprova-ho amb el **Cuentagotas** (**I**).

Recorda que el resultat **depèn de la llum de la foto**, així que el color final pot no ser idèntic al que et van donar.

## <img class="ic" src="svg/ic-palette.svg" alt=""> El color no queda igual que el codi

És normal. El mode **Color** respecta la **llum de la foto**: una sabata molt clara fa que el color quedi massa clar, i una de fosca el fa massa fosc. Es nota sobretot amb la **mostassa** i el **blau marí**. Tens **dues maneres** de solucionar-ho:

- **Opció A:** deixes la capa de **color sólido** i la ajustes amb **Niveles** o **Curvas**.
- **Opció B:** en comptes de la capa de color sólido, fas servir una capa de **Mapa de degradado** (més avall).

### Opció A: Niveles o Curvas

Afegeix una capa d'ajust **Niveles** o **Curvas** i **retalla-la** a la capa de color perquè només actuï sobre la sabata:

- **Retallar a la capa de sota:** **Ctrl + Alt + G** (Windows) o **Cmd + Opción + G** (Mac). O bé fes **clic dret** sobre la capa d'ajust i tria **Crear máscara de recorte**.
- Mou el control del mig (els **grisos**) fins que el to s'assembli al codi.
- Comprova el resultat amb el **Cuentagotas** (**I**): clica sobre la sabata i mira el codi al **Selector de color**.

## <img class="ic" src="svg/ic-mountain.svg" alt=""> Opció B: Mapa de degradado en comptes del color sólido

El mode **Color** conserva la **llum** de la foto. Si la sabata original és **negra o molt fosca**, no hi ha llum que conservar: el color nou **gairebé no es veu** i la sabata continua sent negra o gris fosc. Aquí el **Color sólido + Modo Color** no funciona bé, i **Niveles** tampoc ho arregla del tot.

En aquest cas (o quan l'opció A no et convenç) **substitueixes la capa de color sólido** per un **Mapa de degradado**: una capa d'ajust que **pinta segons la llum de cada píxel**. Les parts fosques agafen un extrem del degradat i les clares, l'altre. Així es **conserven els reflexos i les ombres**, però amb el color nou.

### Pas a pas

1. Amb la **selecció** de la sabata activa: **Capa > Nueva capa de ajuste > Mapa de degradado…**. La selecció es converteix en la **màscara** de la capa.
2. Fes **clic sobre la barra del degradat** al panell **Propiedades** per obrir l'**Editor de degradados**.
3. A la barra hi ha **marcadors de color** (els quadradets de sota). **Doble clic** sobre un marcador per triar-ne el color. Al **Selector de color** escriu el **codi** al camp **#**.
4. Posa **tres marcadors**: un a **l'esquerra** (0 %) amb una versió **més fosca** del color, un al **mig** amb el **color de marca** (el codi), i un a la **dreta** (100 %) amb una versió **més clara**. Per afegir-ne un, clica **a sota** de la barra.
5. Accepta amb **OK** i dona un **nom** a la capa (per exemple `color_mostassa`).

| Marcador | Què pinta | Color |
|---|---|---|
| **Esquerra** (0 %) | Les ombres | El color de marca **més fosc** |
| **Mig** | Els tons mitjans | El **codi de marca** |
| **Dreta** (100 %) | Els reflexos | El color de marca **més clar** |

### Si la sabata continua massa fosca

- **Mou el marcador del mig cap a l'esquerra** (per exemple, al 25 %): així el **codi de marca** apareix també en les zones fosques.
- **No posis negre pur** a l'esquerra: es perd el detall de les costures i les arrugues.
- Retoca la **màscara** amb el **Pincel**, igual que amb la capa de color.
- Si cal, afegeix **Niveles** o **Curvas** retallada a sobre (**Ctrl + Alt + G**, **Cmd + Opción + G**, o clic dret > **Crear máscara de recorte**).

### Quina opció faig servir?

| Si… | Fes servir… |
|---|---|
| El color queda bé o només un pèl clar o fosc | **Color sólido + Modo Color** (+ **Niveles** o **Curvas** si cal: opció A) |
| El color de base és **molt fosc** o no hi ha manera d'ajustar-lo | **Mapa de degradado** en comptes de la capa de color sólido (opció B) |

## <img class="ic" src="svg/ic-warning.svg" alt=""> Errors freqüents

- **Capa de color sense màscara:** pinta tota la foto.
- **Aurèoles** o taques de color a les cames: la selecció era poc fina; retoca la màscara.
- **Esborrar** en comptes de fer màscara: ja no es pot recuperar.
- **Capes sense nom:** després no saps quina és quina.

## <img class="ic" src="svg/ic-pin.svg" alt=""> Per recordar

- Un color de marca es dona amb un **codi hexadecimal** (**#RRGGBB**).
- Capa de **Relleno de color sólido** + **Modo Color** + **màscara**.
- Si el to no coincideix: **Niveles o Curvas retallada** (opció A) o **Mapa de degradado** en comptes del color sólido (opció B).
