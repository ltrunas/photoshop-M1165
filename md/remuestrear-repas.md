# Remuestrear: repàs amb comparativa

Aquesta pàgina és el **repàs del Remuestrear**, que no vam poder treballar a la sessió 6. Si has fet la pràctica d'ajustar la imatge, ja l'has fet servir. Aquí el veiem amb exemples.

## La idea en una frase

**Remuestrear** vol dir que Photoshop **canvia el nombre de píxels** de la imatge. Si n'hi ha més, se n'han d'**inventar** de nous a partir dels que ja hi ha. Això es fa sempre amb un **mètode de càlcul**, i cada mètode dóna un resultat diferent.

## Comparativa: el mateix retall ampliat amb mètodes diferents

![Comparativa de quatre mètodes d'ampliació de la mateixa imatge petita](img/remuestrear-comparativa.png)

La imatge és un tros petit d'una foto (65 × 49 píxels) **ampliat 6 vegades** amb quatre mètodes. Aquesta comparativa està feta amb un programa de càlcul d'imatges (Python), **no amb Photoshop**: serveix per veure la **idea** de cada mètode. Els mètodes de Photoshop tenen els seus propis noms i algoritmes, i els resultats no seran idèntics.

- **Por aproximación (bordes definidos):** copia els píxels sense barrejar-los. Es veuen els **quadradets**, però les vores es mantenen dures. Va bé per a icones o píxel art.
- **Bilineal:** barreja els píxels veïns. El resultat és suau i una mica **borrós**.
- **Bicúbica:** també suavitza, però manté millor les transicions de to.
- **Lanczos:** manté més la sensació de **nitidesa** a les vores.

La conclusió és que **cap mètode afegeix detall real**. Només canvia la manera de repartir els píxels nous.

## Què fem a classe

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
