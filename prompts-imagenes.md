# Prompts de imágenes — El Bestiario del Emprendimiento Latinoamericano

## Cómo usar este documento

1. Abre la ficha de la imagen que quieras generar y copia su bloque JSON completo.
2. Pégalo en tu generador de imágenes (Nano Banana u otro). Cada prompt es autocontenido.
3. Guarda el resultado con el **nombre exacto** de la ficha, dentro de la carpeta `images/` del libro.
4. Recarga el libro: cuando el archivo existe en esa ruta, reemplaza solo al recuadro punteado.

## Estilo común

- **Estilo:** fotorrealista, de aire documental y de gabinete de explorador.
- **Paleta:** `#1a120c` `#f6efdf` `#8a4b12` `#e0a050` `#2f5d57`
- **Mundo visual:** el cuaderno del explorador de la portada: madera oscura, papel envejecido, latón, lámpara de queroseno y mapas de América Latina; en los capítulos de cada figura, la criatura real en su entorno. Luz cálida y baja en todas.

## Portada

### `images/portada.jpg`

- **Uso:** portada del libro (plana, la entregó el autor)
- **Proporción:** 3:4
- **Estado:** lista
- **Descripción:** Portada de El Bestiario del Emprendimiento Latinoamericano

### `images/portada-mockup.jpg`

- **Uso:** portada del libro en mockup 3D (generada con make_mockup.py)
- **Proporción:** 4:3
- **Estado:** lista
- **Descripción:** El libro El Bestiario del Emprendimiento Latinoamericano, con su portada de cuaderno de explorador

## Prólogo — Por qué necesitamos nuevas figuras

### `images/prologo-hero.jpg`

- **Uso:** imagen hero (abre el capítulo)
- **Proporción:** 16:9
- **Estado:** pendiente
- **Descripción:** Un mapa antiguo de América Latina sobre una mesa de madera, iluminado por una lámpara de queroseno

```json
{
  "type": "photorealistic photograph",
  "subject": "Un mapa antiguo de América Latina extendido sobre una mesa de madera oscura, con una lámpara de queroseno encendida a un lado y una brújula de latón.",
  "setting": "Gabinete de explorador al amanecer, cuarto en penumbra.",
  "composition": "Plano amplio horizontal, mapa en el tercio inferior, aire oscuro arriba.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 35 mm, f/2.8.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Misterio tranquilo, comienzo de un viaje.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "16:9",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/prologo-1.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Una brújula de latón sobre un mapa dibujado a mano que no coincide con el terreno de la mesa

```json
{
  "type": "photorealistic photograph",
  "subject": "Una brújula de latón sobre un mapa dibujado a mano de otro país cuyos trazos no coinciden con la madera de la mesa.",
  "setting": "Mesa de trabajo, luz de lámpara desde la izquierda.",
  "composition": "Plano cerrado cenital ligeramente inclinado, brújula en el tercio derecho.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 50 mm, f/2.8.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Desajuste, duda.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

## Capítulo 1 — El bestiario global (y sus límites)

### `images/bestiario-global-hero.jpg`

- **Uso:** imagen hero (abre el capítulo)
- **Proporción:** 16:9
- **Estado:** pendiente
- **Descripción:** Vitrina antigua de gabinete con estatuillas de bronce de un unicornio, una gacela, una cebra y un camello

```json
{
  "type": "photorealistic photograph",
  "subject": "Una vitrina antigua de gabinete con estatuillas de bronce de un unicornio, una gacela, una cebra y un camello, alineadas en repisas.",
  "setting": "Sala de museo pequeña, vidrios con reflejos tenues, madera oscura.",
  "composition": "Plano frontal amplio, vitrina centrada con aire a los lados.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 35 mm, f/4.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Respeto por lo heredado, distancia.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "16:9",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/bestiario-global-1.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Cuaderno de campo abierto con bocetos a tinta de una gacela y una cebra

```json
{
  "type": "photorealistic photograph",
  "subject": "Un cuaderno de campo abierto con bocetos a tinta de una gacela y una cebra, junto a una pluma y un frasco de tinta.",
  "setting": "Escritorio de madera, luz ámbar lateral.",
  "composition": "Plano cerrado desde arriba, cuaderno en diagonal.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 50 mm, f/2.8.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Observación paciente.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/bestiario-global-2.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** El borde de un mapa antiguo desplegado: el papel termina, pero la mesa de madera sigue

```json
{
  "type": "photorealistic photograph",
  "subject": "El borde de un mapa antiguo desplegado sobre una mesa: el papel termina y la madera vacía sigue más allá.",
  "setting": "Cuarto en penumbra, luz de lámpara que cae sobre el borde del papel.",
  "composition": "Plano medio bajo, borde del mapa cruzando en diagonal, espacio vacío a la derecha.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 50 mm, f/2.8.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Frontera, límite.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

## Capítulo 2 — Cuando la promesa ocupa el lugar del aprendizaje

### `images/promesa-aprendizaje-hero.jpg`

- **Uso:** imagen hero (abre el capítulo)
- **Proporción:** 16:9
- **Estado:** pendiente
- **Descripción:** Un velero pequeño navegando de noche entre la niebla hacia una luz lejana

```json
{
  "type": "photorealistic photograph",
  "subject": "Un velero pequeño de madera navegando de noche entre la niebla hacia una luz lejana y cálida.",
  "setting": "Mar en calma, cielo nocturno con bruma, luz ámbar en el horizonte.",
  "composition": "Plano amplio, velero pequeño en el tercio izquierdo, luz en el derecho.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 35 mm, f/2.8, exposición larga suave.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Atracción serena, algo de peligro.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "16:9",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/promesa-aprendizaje-1.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Una pequeña sirena tallada en madera y conchas sobre un mapa náutico antiguo

```json
{
  "type": "photorealistic photograph",
  "subject": "Una pequeña sirena tallada en madera, rodeada de conchas, sobre un mapa náutico antiguo.",
  "setting": "Mesa de capitán, luz de lámpara.",
  "composition": "Plano cerrado, sirena en el tercio derecho, fondo suave.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 85 mm, f/2.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Seducción y misterio.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/promesa-aprendizaje-2.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Un telescopio de latón sobre la cubierta de un velero apuntando hacia el horizonte en calma

```json
{
  "type": "photorealistic photograph",
  "subject": "Un telescopio de latón sobre la cubierta de un velero, apuntando al horizonte en calma.",
  "setting": "Cubierta de madera al atardecer, mar quieto.",
  "composition": "Plano medio de perfil, telescopio en diagonal.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 50 mm, f/2.8.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Vigilancia, criterio.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

## Capítulo 3 — El valor que el sistema no sabe leer

### `images/valor-invisible-hero.jpg`

- **Uso:** imagen hero (abre el capítulo)
- **Proporción:** 16:9
- **Estado:** pendiente
- **Descripción:** Un cisne blanco emergiendo de la neblina en un lago al amanecer, lejos de la orilla

```json
{
  "type": "photorealistic photograph",
  "subject": "Un cisne blanco emergiendo de la neblina en un lago, lejos de la orilla.",
  "setting": "Lago al amanecer, niebla baja, luz ámbar tenue.",
  "composition": "Plano amplio, cisne pequeño en el tercio derecho, mucho aire.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 70 mm, f/4.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Silencio, valor que apenas se insinúa.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "16:9",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/valor-invisible-1.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Un cisne blanco nadando de perfil en un lago tranquilo, con reflejos suaves en el agua

```json
{
  "type": "photorealistic photograph",
  "subject": "Un cisne blanco nadando de perfil con reflejos suaves en el agua tranquila.",
  "setting": "Lago sereno, luz lateral cálida.",
  "composition": "Plano medio horizontal, cisne en el tercio izquierdo.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 135 mm, f/4.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Calma, elegancia discreta.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/valor-invisible-2.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Una lupa de latón sobre un mapa de América Latina, enfocando una zona pequeña

```json
{
  "type": "photorealistic photograph",
  "subject": "Una lupa de latón sobre un mapa de América Latina, enfocando una zona pequeña.",
  "setting": "Escritorio de madera, luz de lámpara.",
  "composition": "Plano cerrado cenital, lupa en el tercio derecho.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 50 mm, f/2.8.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Mirar mejor.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

## Capítulo 4 — La lógica real de supervivencia

### `images/supervivencia-hero.jpg`

- **Uso:** imagen hero (abre el capítulo)
- **Proporción:** 16:9
- **Estado:** pendiente
- **Descripción:** Un colibrí en vuelo estacionario frente a una flor roja en un bosque tropical con neblina

```json
{
  "type": "photorealistic photograph",
  "subject": "Un colibrí en vuelo estacionario frente a una flor roja.",
  "setting": "Bosque tropical de montaña con neblina, luz de amanecer ámbar.",
  "composition": "Plano amplio, colibrí en el tercio izquierdo, follaje desenfocado.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 200 mm, f/4, velocidad alta.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Persistencia pequeña, vida.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "16:9",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/supervivencia-1.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Un colibrí en vuelo estacionario recogiendo una gota de agua de una hoja, en primer plano

```json
{
  "type": "photorealistic photograph",
  "subject": "Un colibrí en vuelo cerca de una hoja con una gota de agua en el borde, en primer plano.",
  "setting": "Selva húmeda, luz suave filtrada.",
  "composition": "Plano cerrado, gota y pico en el tercio derecho.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente macro de 100 mm, f/3.5.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Gesto mínimo, constancia.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

## Capítulo 5 — Capital que entiende el viaje

### `images/capital-viaje-hero.jpg`

- **Uso:** imagen hero (abre el capítulo)
- **Proporción:** 16:9
- **Estado:** pendiente
- **Descripción:** Un delfín saltando sobre el mar abierto al amanecer

```json
{
  "type": "photorealistic photograph",
  "subject": "Un delfín saltando sobre el mar abierto, con gotas de agua en el aire.",
  "setting": "Mar al amanecer, cielo ámbar y azul profundo.",
  "composition": "Plano amplio, delfín en el tercio derecho, horizonte bajo.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 200 mm, f/5.6, velocidad alta.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Compañía, energía amable.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "16:9",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/capital-viaje-1.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Dos delfines nadando junto a una pequeña lancha de madera en aguas tranquilas

```json
{
  "type": "photorealistic photograph",
  "subject": "Dos delfines nadando junto a una pequeña lancha de madera.",
  "setting": "Aguas tranquilas, luz suave de la mañana.",
  "composition": "Plano medio desde la lancha, delfines en el tercio izquierdo.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 70 mm, f/4.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Acompañar sin imponer.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/capital-viaje-2.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Vista aérea del mar: una franja de aguas claras y poco profundas junto a una zona de agua azul oscuro y profunda

```json
{
  "type": "photorealistic photograph",
  "subject": "Vista aérea del mar: una franja de aguas claras y poco profundas junto a una zona de agua azul oscuro y profunda.",
  "setting": "Costa tropical, luz alta de la mañana.",
  "composition": "Plano cenital amplio, línea de contraste en diagonal.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Dron, lente de 24 mm, f/5.6.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Cada cosa en su momento.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

## Capítulo 6 — Un sistema, no una competencia

### `images/sistema-hero.jpg`

- **Uso:** imagen hero (abre el capítulo)
- **Proporción:** 16:9
- **Estado:** pendiente
- **Descripción:** Un auditorio vacío con atriles de orquesta y partituras iluminados por luz cálida

```json
{
  "type": "photorealistic photograph",
  "subject": "Un auditorio vacío con atriles de orquesta y partituras iluminados por luz cálida, sin texto legible.",
  "setting": "Sala de conciertos tenue, madera y terciopelo oscuro.",
  "composition": "Plano amplio desde el escenario, atriles en primer plano, butacas al fondo.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 35 mm, f/2.8.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Orden previo a la música.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "16:9",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/sistema-1.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Vista aérea de cuatro ríos que se unen en un solo cauce dentro de la selva

```json
{
  "type": "photorealistic photograph",
  "subject": "Vista aérea de cuatro ríos que se unen en un solo cauce dentro de la selva.",
  "setting": "Selva tropical, luz suave de la mañana.",
  "composition": "Plano cenital amplio, confluencia en el centro.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Dron, lente de 24 mm, f/5.6.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Funciones distintas, un mismo cauce.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/sistema-2.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** La mano de un director de orquesta con una batuta frente a atriles iluminados, con los músicos desenfocados

```json
{
  "type": "photorealistic photograph",
  "subject": "La mano de un director de orquesta con una batuta frente a atriles iluminados, con los músicos desenfocados.",
  "setting": "Escenario con luz cálida.",
  "composition": "Plano medio cerrado, mano y batuta en el tercio izquierdo.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 85 mm, f/2.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Coordinar, sin controlar.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

## Capítulo 7 — Del lenguaje a la práctica

### `images/practica-hero.jpg`

- **Uso:** imagen hero (abre el capítulo)
- **Proporción:** 16:9
- **Estado:** pendiente
- **Descripción:** Escritorio de campo con una libreta abierta, una lupa, una brújula y una lámpara encendida

```json
{
  "type": "photorealistic photograph",
  "subject": "Un escritorio de campo con una libreta abierta (páginas sin texto legible), una lupa, una brújula y una lámpara encendida.",
  "setting": "Mesa de madera, luz ámbar de lámpara.",
  "composition": "Plano amplio, objetos repartidos con aire oscuro arriba.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 35 mm, f/2.8.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Del lenguaje a la acción.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "16:9",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/practica-1.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Una brújula de latón sobre una libreta abierta con las páginas en blanco

```json
{
  "type": "photorealistic photograph",
  "subject": "Una brújula de latón sobre una libreta abierta con las páginas en blanco.",
  "setting": "Escritorio de madera, luz lateral cálida.",
  "composition": "Plano cerrado cenital, brújula en el centro-derecha.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 50 mm, f/2.8.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Orientación.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/practica-2.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Dos personas conversando de espaldas en un café de barrio, con dos tazas sobre la mesa

```json
{
  "type": "photorealistic photograph",
  "subject": "Dos personas conversando, vistas de espaldas, en un café de barrio, con dos tazas sobre la mesa.",
  "setting": "Café con luz de la tarde entrando por la ventana.",
  "composition": "Plano medio desde atrás, personas en el tercio izquierdo.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 35 mm, f/2.8.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Acompañar es sostener.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

## Capítulo 8 — Hacia un ecosistema que aprende

### `images/ecosistema-hero.jpg`

- **Uso:** imagen hero (abre el capítulo)
- **Proporción:** 16:9
- **Estado:** pendiente
- **Descripción:** Un bosque de montaña al amanecer con luz atravesando la neblina y plantas jóvenes bajo los árboles

```json
{
  "type": "photorealistic photograph",
  "subject": "Un bosque de montaña al amanecer, con rayos de luz atravesando la neblina y plantas jóvenes bajo los árboles.",
  "setting": "Bosque nublado latinoamericano.",
  "composition": "Plano amplio, árboles en los lados, claro de luz al centro.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 35 mm, f/5.6.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Un sistema que aprende.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "16:9",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/ecosistema-1.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Un brote joven creciendo entre hojas secas en el suelo de un bosque, con luz suave

```json
{
  "type": "photorealistic photograph",
  "subject": "Un brote joven creciendo entre hojas secas en el suelo de un bosque.",
  "setting": "Suelo de bosque, luz suave y tenue.",
  "composition": "Plano cerrado, brote en el tercio derecho.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente macro de 100 mm, f/3.5.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Lo aprendido que no se desperdicia.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

## Epílogo — Leer con otros ojos

### `images/epilogo-hero.jpg`

- **Uso:** imagen hero (abre el capítulo)
- **Proporción:** 16:9
- **Estado:** pendiente
- **Descripción:** Una persona de espaldas entra en una sala oscura con una linterna encendida

```json
{
  "type": "photorealistic photograph",
  "subject": "Una persona de espaldas entra en una sala oscura con una linterna encendida.",
  "setting": "Sala vacía de una casa antigua, penumbra.",
  "composition": "Plano amplio, figura pequeña en el tercio izquierdo.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 35 mm, f/2.8.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Cambio de mirada.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "16:9",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/epilogo-1.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Una linterna encendida sobre un mapa antiguo en una habitación en penumbra

```json
{
  "type": "photorealistic photograph",
  "subject": "Una linterna encendida sobre un mapa antiguo en una habitación en penumbra.",
  "setting": "Mesa de madera, único foco de luz.",
  "composition": "Plano medio bajo, linterna en el tercio derecho.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 50 mm, f/2.8.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Leer con otros ojos.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

## Diagnóstico — Tu mapa del Bestiario

### `images/mapa-figuras-hero.jpg`

- **Uso:** imagen hero (abre el capítulo)
- **Proporción:** 16:9
- **Estado:** pendiente
- **Descripción:** Una pluma, una brújula, una lupa y una lámpara sobre un escritorio de madera

```json
{
  "type": "photorealistic photograph",
  "subject": "Una pluma fuente, una brújula, una lupa y una lámpara sobre un escritorio de madera.",
  "setting": "Gabinete del explorador, luz ámbar.",
  "composition": "Plano amplio, objetos en fila suave con aire arriba.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 35 mm, f/4.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Cuatro lentes para mirarse.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "16:9",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```

### `images/mapa-figuras-1.jpg`

- **Uso:** imagen de apoyo dentro del texto
- **Proporción:** 3:2
- **Estado:** pendiente
- **Descripción:** Un cuaderno abierto con una pluma fuente sobre una página en blanco, junto a una lámpara

```json
{
  "type": "photorealistic photograph",
  "subject": "Un cuaderno abierto con una pluma fuente sobre una página en blanco, junto a una lámpara.",
  "setting": "Escritorio de madera, luz cálida.",
  "composition": "Plano cerrado cenital, cuaderno en diagonal.",
  "lighting": "Luz cálida y baja, de lámpara de queroseno o de amanecer ámbar, con sombras suaves y una leve niebla",
  "camera": "Full frame, lente de 50 mm, f/2.8.",
  "color_palette": [
    "#1a120c",
    "#f6efdf",
    "#8a4b12",
    "#e0a050",
    "#2f5d57"
  ],
  "mood": "Listo para anotar.",
  "style": "Fotografía editorial realista de aire documental, texturas naturales (papel envejecido, latón, madera), grano fino, sin apariencia de ilustración ni de render 3D",
  "aspect_ratio": "3:2",
  "avoid": [
    "texto legible",
    "letras",
    "logos",
    "marcas de agua",
    "bordes o marcos",
    "rostros deformes",
    "aspecto de foto de stock posada"
  ]
}
```
