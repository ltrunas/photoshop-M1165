# Calcular píxels pas a pas

Quan et donen una mida en **centímetres** o **polzades** i una **resolució en ppp**, has de saber **quants píxels** necessites. Aquesta pàgina t'ho explica pas a pas. És la base de la **pràctica d'ajustar la imatge**.

## 🧮 La fórmula

![De centímetres a píxels en tres passos](svg/formula-pixels.svg)

**píxels = (mida en cm ÷ 2,54) × resolució en ppp**

Una polzada (*inch*) són **2,54 cm**. Per això dividim per 2,54 abans de multiplicar.

## 📋 Dos casos

### 📱 Et donen la mida en píxels (pantalla)

No cal calcular res. Per exemple, una publicació vertical d'Instagram és de **1080 × 1350 píxels**. Només has de fer coincidir la imatge amb aquests valors.

### 🖨️ Et donen la mida en centímetres (impressió)

Has de calcular l'**ample** i l'**alçada** per separat.

**Exemple: una portada A4 (21 × 29,7 cm) a 300 ppp**

| | Càlcul | Resultat |
|---|---|---|
| Ample | (21 ÷ 2,54) × 300 | ≈ **2480 px** |
| Alçada | (29,7 ÷ 2,54) × 300 | ≈ **3508 px** |

## 🧮 Calculadora de píxels

**Primer fes-ho tu a mà** amb la fórmula. Després **comprova els teus càlculs** amb la calculadora:

<iframe id="calc-frame" src="calculadora.html?embed=1" title="Calculadora de píxels" style="width:100%;height:820px;border:0;border-radius:14px;background:transparent" loading="lazy"></iframe>

💡 La calculadora t'ajuda a **comprovar**, però al document de justificació has d'**escriure els passos**. També la tens a pantalla completa: [obre la calculadora](calculadora.html).

## 🪜 Els passos de cada versió

1. **Calcula** la mida final en píxels.
2. **Retalla** amb l'eina **Recortar** (**C**) amb la **proporció** de l'encàrrec. Mira la pàgina **Retalls bàsics**.
3. **Ajusta** la mida a **Imagen > Tamaño de la imagen** (**Ctrl + Alt + I**, **Cmd + Opción + I** a Mac) amb els píxels i els ppp calculats.

## ⚖️ Compara abans de continuar

Mira els píxels que té la imatge **després de retallar** i compara'ls amb els que necessites:

- 📉 **Tens més píxels dels que necessites:** estàs **reduint**. No hi ha problema de qualitat.
- 📈 **Tens menys píxels dels que necessites:** estàs **ampliant**. Photoshop ha d'**inventar píxels** (**Remuestrear**) i perdràs nitidesa. Tria bé el mètode: mira la pàgina **Remuestrear: repàs amb comparativa**.

## ✅ Comprova el resultat

Quan acabis, a **Tamaño de la imagen** han de sortir **exactament** els valors que has calculat.
