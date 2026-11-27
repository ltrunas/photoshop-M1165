# Canviar el fons i integrar l'ombra

Canviar el fons no és només retallar i enganxar. Perquè la imatge sigui **creïble**, el subjecte ha de **lligar** amb el fons: les vores netes, la perspectiva correcta i, sobretot, **una ombra** que el fixi al terra.

## <img class="ic" src="svg/ic-image.svg" alt=""> L'ordre de capes

Aquest és l'ordre de capes que hauries de tenir al final de la pràctica.

![Ordre de capes: colors, ombra, persona amb màscara, fons nou i Fondo intacte](svg/capes-sabatilles.svg)

## <img class="ic" src="svg/ic-steps.svg" alt=""> Pas a pas

1. **Duplica el Fondo** un altre cop i anomena la capa `persona`. Selecciona la persona i les sabates amb **Selección > Sujeto**.
2. Retoca la selecció amb **Seleccionar y aplicar máscara…** (vegeu més avall) i converteix-la en **màscara de capa**. El fons blau queda **transparent**.
3. Porta el fons nou a la imatge: **Archivo > Colocar incrustado…**. Ajusta'l amb **Edición > Transformación libre** (**Ctrl + T** a Windows, **Cmd + T** a Mac) i col·loca'l **per sota** de la persona.
4. Posa-hi l'**ombra** (vegeu més avall).
5. Escull el **color de sabata** que quedi millor amb el fons.

## <img class="ic" src="svg/ic-wrench.svg" alt=""> Perfeccionar la selecció: Seleccionar y aplicar máscara

Un cop has fet la selecció amb **Selección de objetos** (**W**) i, si cal, el **Lazo** (**L**), no la converteixis directament en màscara. Obre l'espai de treball de perfeccionament: **Seleccionar y aplicar máscara…** (al menú **Selección** o amb el botó de la barra d'opcions). S'obre una finestra a part, pensada per **repassar les vores**.

![Espai de treball Seleccionar y aplicar máscara: la sabatilla sobre fons transparent i el panell Propiedades a la dreta](img/seleccionar-aplicar-mascara.jpg)

### Com es treballa

1. **Mira bé la vora:** amb la **Lupa** (**Z**) fes zoom a les zones difícils (la sola, els cordons, la pell).
2. Amb el **Pincel** de perfeccionar, **passa'l per les vores** que no han quedat bé: afegeix a la selecció el que falta.
3. Mantén **Alt** (**Opción** a Mac) i pinta per **restar** el que no volies: la pell, el fons, les aurèoles.
4. Fes servir els **valors del panell de la dreta** per suavitzar la vora (vegeu la taula).
5. A **Enviar a** tria com vols el resultat (per exemple, **Máscara de capa**) i prem **OK**.

### Els valors del panell de la dreta (Propiedades)

![Panell Propiedades de Seleccionar y aplicar máscara](img/seleccionar-aplicar-mascara-propietats.jpg)

| Valor | Què fa |
|---|---|
| **Transparencia** | Només canvia **com veus** el fons (més o menys transparent) per revisar la vora. No canvia la selecció. |
| **Radio** | Mida de la zona de la vora que Photoshop analitza. Ajuda amb **vores difícils**, com els cabells o els cordons. |
| **Suavizado** | **Arrodoneix** les vores dentades. |
| **Suavizar** | Fa la vora **més difuminada**. Si en poses molta, la sabata sembla desenfocada. |
| **Contraste** | **Endureix** la vora. Va bé per treure una vora massa tova. |
| **Desplazamiento de borde** | Valors **negatius** encongeixen la selecció (treuen aurèoles); valors **positius** l'amplien. |
| **Descontaminar colores** | Treu el color del fons que queda enganxat a la vora. |
| **Enviar a** | On va el resultat: **Selección**, **Máscara de capa**, una capa nova… |

Mou els valors **a poc a poc** i mira la vora amb zoom. Si t'has passat, el botó de **restaurar** de baix a l'esquerra torna als valors inicials. Si la vora no queda bé amb els valors, **repassa-la amb el pincel** abans d'acceptar.

Per veure millor el resultat, canvia el **Modo de vista** (la miniatura **Vista**): sobre **transparent** es veuen els defectes; sobre **blanc** o **negre** es veuen les aurèoles. **Mostrar borde (J)** i **Mostrar original (P)** ajuden a comparar.

## <img class="ic" src="svg/ic-fog.svg" alt=""> L'ombra de contacte

Sense ombra, la persona **sembla enganxada**, com si flotés sobre el fons. Una ombra senzilla ho arregla:

1. Crea una **capa nova entre el fons i la persona** i anomena-la `ombra`.
2. Amb el **Pincel** (**B**) en **negre**, **Dureza 0 %** i **Opacidad 30-40 %**, pinta una taca **on el cos toca el terra**.
3. Posa l'ombra **cap al costat contrari de la llum** del fons. Per exemple, si la llum ve de dalt a la dreta, l'ombra va cap a l'esquerra i cap avall.
4. Suavitza-la: **Filtro > Desenfocar > Desenfoque gaussiano…**.
5. Posa la capa en **Modo de fusión: Multiplicar**, perquè l'ombra enfosqueixi el fons sense tapar-lo.

## <img class="ic" src="svg/ic-eye.svg" alt=""> Perquè el fons "encaixi"

- **Perspectiva:** el fons ha de mirar-se des de la mateixa altura que la foto. Si no, la persona sembla en un altre món.
- **Llum:** la direcció de la llum del fons ha de coincidir amb la de la foto.
- **Vores:** una vora massa dura s'ha de suavitzar amb **Calar** o amb el pincel.
- **Escala:** ajusta la mida del fons perquè la persona no sigui gegant ni minúscula.

## <img class="ic" src="svg/ic-pin.svg" alt=""> Per recordar

- **No tocis mai el Fondo original.**
- **Persona amb màscara**, fons a sota i **ombra entre els dos**.
- Ombra: **pincel suau**, **Desenfoque gaussiano**, **Multiplicar**.
