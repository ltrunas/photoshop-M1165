# Selecció i màscares

Una **selecció** és una zona de la imatge on actuarà el que facis després (pintar, omplir, aplicar un ajust, esborrar). Una **màscara** és una manera de **amagar parts d'una capa sense esborrar-les**, i per això és **no destructiva**.

## El menú Selección

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

## Les eines de selecció

| Eina | Drecera | Per a què serveix |
|---|---|---|
| **Marco** | M | Selecció rectangular o el·líptica |
| **Lazo** | L | Selecció a mà alçada, o per punts amb el Lazo poligonal |
| **Selección de objetos** | W | Seleccionar un objecte o una persona de manera ràpida |

**Trucs amb el Marco:** **Maj** per fer un quadrat o un cercle perfecte, i **Alt** (**Opción** a Mac) per dibuixar des del centre.

### Sumar, restar i intersecar

A la barra de **opciones** hi ha quatre botons que controlen com es combina una selecció nova amb l'anterior:

- **Nueva selección:** substitueix l'anterior.
- **Añadir a la selección:** suma. Es pot fer amb **Maj** premut.
- **Restar de la selección:** treu. Es pot fer amb **Alt** (**Opción**) premut.
- **Intersección:** es queda només la part comuna.

## Retocar una selecció

Amb una selecció activa, **Selección > Modificar** permet:

- **Ampliar** o **Reducir** la selecció uns píxels.
- **Suavizar** les vores.
- **Calar** (*feather*): difumina la vora perquè la transició no sigui dura. És important perquè una vora massa dura sembla retallada.

## Què és una màscara de capa

Una **màscara de capa** és una imatge en **blanc, negre i grisos** enganxada a una capa. Fixa't en aquesta regla, perquè és tot el que cal recordar:

| Color a la màscara | Què passa a la capa |
|---|---|
| **Blanc** | Es **veu** |
| **Negre** | Està **amagat** |
| **Gris** | Es veu **a mitges** (transparència parcial) |

**Per què és millor que esborrar?** Perquè no es perd cap píxel. Si t'equivoques, pintes de blanc i el que s'havia amagat torna a aparèixer. És el mateix concepte que el retall no destructiu: es pot **rectificar**.

### Com es crea

1. Selecciona la capa al panell **Capas**.
2. Fes una selecció de la part que vols **mantenir** (per exemple, amb **Selección de objetos** o **Sujeto**).
3. Clica el botó de **màscara** de baix del panell **Capas** (el rectangle amb un cercle). La part seleccionada es veu i la resta s'amaga.

També pots fer-ho amb **Capa > Máscara de capa**, que ofereix opcions com *Mostrar todo* i *Ocultar todo*.

### Retocar la màscara amb el pinzell

1. Clica la **miniatura de la màscara** (apareix un marc al voltant).
2. Tria el **Pincel** (**B**).
3. Pinta de **negre** per amagar i de **blanc** per tornar a mostrar.
4. Prem **X** per **intercanviar** negre i blanc, i **D** per tornar als colors per defecte.

### Altres operacions

| Què vols fer | Com |
|---|---|
| Veure només la màscara | **Alt** (**Opción**) + clic a la miniatura |
| Desactivar la màscara temporalment | **Maj** + clic a la miniatura |
| Moure la imatge sense moure la màscara | Clica la **cadena** entre la capa i la màscara per desvincular-les |
| Aplicar l'efecte a tot el document | Prova una **capa d'ajust**, que porta màscara |

## Exercici de classe (proposta)

1. Obre una foto amb una persona o un objecte clar i duplica la capa de fons.
2. Selecciona el subjecte amb **Selección > Sujeto** i retoca-ho amb Sumar i Restar.
3. Crea una màscara de capa i col·loca un **fons nou** a sota.
4. Arregla les vores amb el **Pincel** en negre i blanc.
5. Guarda en **PSD** amb les capes i la màscara.

## Per recordar

- Una **selecció** limita on actua el que fas.
- Una **màscara** amaga sense esborrar: **blanc = es veu, negre = amagat**.
- Si dubtes, **màscara abans que esborrar**.
