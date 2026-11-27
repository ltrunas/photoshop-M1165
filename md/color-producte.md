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

## <img class="ic" src="svg/ic-palette.svg" alt=""> El color no queda igual que el codi

És normal. El mode **Color** respecta la **llum de la foto**: una sabata molt clara fa que el color quedi massa clar, i una de fosca el fa massa fosc. Es nota sobretot amb la **mostassa** i el **blau marí**.

Per corregir-ho, afegeix una capa d'ajust **Niveles** o **Curvas** i **retalla-la** a la capa de color perquè només actuï sobre la sabata:

- **Retallar a la capa de sota:** **Ctrl + Alt + G** (Windows) o **Cmd + Opción + G** (Mac).
- Mou el control del mig (els **grisos**) fins que el to s'assembli al codi.
- Comprova el resultat amb el **Cuentagotas** (**I**): clica sobre la sabata i mira el codi al **Selector de color**.

## <img class="ic" src="svg/ic-warning.svg" alt=""> Errors freqüents

- **Capa de color sense màscara:** pinta tota la foto.
- **Aurèoles** o taques de color a les cames: la selecció era poc fina; retoca la màscara.
- **Esborrar** en comptes de fer màscara: ja no es pot recuperar.
- **Capes sense nom:** després no saps quina és quina.

## <img class="ic" src="svg/ic-pin.svg" alt=""> Per recordar

- Un color de marca es dona amb un **codi hexadecimal** (**#RRGGBB**).
- Capa de **Relleno de color sólido** + **Modo Color** + **màscara**.
- Si el to no coincideix: **Niveles o Curvas retallada**.
