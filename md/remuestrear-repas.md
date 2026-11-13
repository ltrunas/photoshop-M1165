# Remuestrear: repàs amb comparativa

Aquesta pàgina és el **repàs del Remuestrear**, que no vam poder treballar a la sessió 6. La necessites per a la **pràctica d'ajustar la imatge**. Llegeix-la abans de començar.

## La idea en una frase

**Remuestrear** vol dir que Photoshop **canvia el nombre de píxels** de la imatge. Si n'hi ha més, se n'han d'**inventar** de nous a partir dels que ja hi ha. Això es fa sempre amb un **mètode de càlcul**, i cada mètode dóna un resultat diferent.

## Comparativa: el mateix retall ampliat amb mètodes diferents

![Comparativa de quatre mètodes d'ampliació de la mateixa imatge petita](img/remuestrear-comparativa.png)

La imatge és el **cim d'una muntanya** (36 × 27 píxels, molt petita) **ampliada 10 vegades** amb quatre mètodes. Està feta amb un programa de càlcul d'imatges (Python), **no amb Photoshop**: serveix per veure la **idea** de cada mètode. Els mètodes de Photoshop tenen els seus propis noms i algoritmes, i els resultats no seran idèntics.

## 🔍 En què t'has de fixar a cada una

**Fixa't sempre en la mateixa zona: la vora del cim contra el cel.** Allà és on es nota la diferència, perquè hi ha un canvi brusc de fosc a clar.

| Mètode | 👀 Què veus a la vora del cim | 🧠 Què fa |
|---|---|---|
| **1. Por aproximación** | **Quadradets** ben marcats, amb les vores dures i esglaonades. No hi ha cap tó intermedi | Copia cada píxel tal qual, sense barrejar |
| **2. Bilineal** | La vora és **la més borrosa**. El cim perd contrast i els detalls es difuminen | Fa la mitjana dels 4 píxels veïns |
| **3. Bicúbica** | **Més suau que els quadradets** i amb transicions de to més naturals. La vora és una mica més definida que a la Bilineal | Mira els 16 píxels veïns i fa una mitjana més intel·ligent |
| **4. Lanczos** | La vora és **la més marcada** i es nota més contrast entre el cim i el cel. Si ampliem molt, pot aparèixer una **aurèola** clara al voltant de les vores | Fa servir encara més píxels veïns i accentua el contrast de les vores |

⚠️ Les diferències entre els mètodes **2, 3 i 4 són subtils**, perquè tots tres suavitzen. Per veure-les, **amplia el dibuix al 200 %** o compara'ls un al costat de l'altre i mira només la vora del cim. La gran diferència és entre el **1** (quadradets) i la resta (suavitzats).

### 📋 Resum

- **Quadradets i vores dures →** *Por aproximación*. Útil per a icones i píxel art.
- **Suau i una mica borrós →** *Bilineal*.
- **Suau, equilibrat →** *Bicúbica*.
- **Més nítid, però amb risc d'aurèoles →** *Lanczos* (a Photoshop s'assembla a **Bicúbica más enfocada**).

La conclusió és que **cap mètode afegeix detall real**. Només canvia la manera de repartir els píxels nous.

## 🪟 On és el Remuestrear a Photoshop

Ho trobaràs a **Imagen > Tamaño de la imagen** (**Ctrl + Alt + I**, **Cmd + Opción + I** a Mac):

![Quadre Tamaño de imagen amb la casella Remuestrear i el seu desplegable obert](img/tamany-imatge.png)

Fixa't en aquestes peces del quadre:

| Peça | Què és |
|---|---|
| **Dimensiones** | La mida actual en píxels (aquí, 1080 px × 1440 px) |
| **Anchura** i **Altura** | Els píxels (o cm, polzades…) que vols. Tria la unitat al desplegable del costat: **Píxeles**, **Centímetros**… |
| **La cadena** (entre Anchura i Altura) | Si és activa, la **proporció** es manté: si canvies l'ample, l'alçada canvia sola. Desactiva-la només si vols deformar |
| **Resolución** | Els **ppp** (aquí, 72 **Píxeles/pulgada**) |
| **Remuestrear** | La casella. **Activada:** pots canviar els píxels. **Desactivada:** només canvies la mida impresa i els píxels es queden igual |
| **El desplegable** de Remuestrear | El mètode, amb les dreceres **Opción + 1** a **Opción + 8** (**Alt + 1** a **8** a Windows) |

💡 **Compara amb la teva comparativa:** el **Bilineal** de Photoshop és el mateix concepte que el 2; la **Bicúbica (degradados suaves)** és la família del 3; **Bicúbica más enfocada (reducción)** es posa per reduir, amb la vora marcada; i **Por aproximación (bordes definidos)** és el dels quadradets.

## Prova-ho tu mateix

1. Obre una de les imatges de la pràctica i duplica la capa de fons (**Ctrl + J**, **Cmd + J** a Mac).
2. Ves a **Imagen > Tamaño de la imagen** (**Ctrl + Alt + I**, **Cmd + Opción + I**).
3. Fixa la unitat a **Píxeles**, activa **Remuestrear** i **amplia l'Anchura al doble**. Prova **Automático**, després **Conservar detalles 2.0** i després **Por aproximación**. Entre prova i prova, torna enrere amb el panell **Historia**.
4. Amplia al **200 %** i compara les vores, el cel i la pell.
5. Fes el mateix **reduint**, amb **Bicúbica más enfocada (reducción)**.

## Preguntes per pensar

- Quin mètode triaries per a una foto que s'ha d'imprimir més gran? I per a un logo d'uns quants píxels?
- Per què la mateixa opció no va bé per ampliar i per reduir?
- Què passa si amplies i redueixes diverses vegades la mateixa imatge?
- Per què és millor **buscar l'original amb més píxels** abans d'ampliar?

Les opcions del desplegable amb el seu detall són a la pàgina **Resolució**.
