---
title: min-block-size
slug: Web/CSS/min-block-size
translation_of: Web/CSS/min-block-size
---
{{CSSRef}}{{SeeCompatTable}}

La propiedad de [CSS](/es/docs/Web/CSS) **`min-block-size`** define el tamaño mínimo horizontal o vertical de un elemento de bloque, dependiendo de los modos de escritura. Esto corresponde ya sea a la propiedad {{cssxref("min-width")}} o a la propiedad {{cssxref("min-height")}}, dependiendo del valor de {{cssxref("writing-mode")}}.

{{EmbedInteractiveExample("pages/css/min-block-size.html")}}

## Sintaxis

```css
/* <length> values */
min-block-size: 100px;
min-block-size: 5em;

/* <percentage> values */
min-block-size: 10%;

/* Keyword values */
min-block-size: max-content;
min-block-size: min-content;
min-block-size: fit-content;
min-block-size: fill-available;

/* Global values */
min-block-size: inherit;
min-block-size: initial;
min-block-size: unset;
```

Si el modo de escritura es verticalmente orientado, el valor de `min-block-size` se relaciona con el mínimo ancho del elemento; de otra manera, se relaciona al mínimo alto del elemento. Una propiedad relacionada es {{cssxref("min-inline-size")}}, que define la otra dimensión del elemento.

{{cssinfo}}

### Valores

La propiedad `min-block-size` toma los mismos valores de las propiedades {{cssxref("min-width")}} y {{cssxref("min-height")}}.

### Sintaxis formal

{{csssyntax}}

## Ejemplo

### Contenido HTML

```html
<p class="exampleText">Example text</p>
```

### Contenido CSS

```css
.exampleText {
  writing-mode: vertical-rl;
  background-color: yellow;
  min-block-size: 200px;
}
```

{{EmbedLiveSample("Ejemplo")}}

## Especificación

| Especificación                                                                                                   | Estado                                           | Comentario          |
| ---------------------------------------------------------------------------------------------------------------- | ------------------------------------------------ | ------------------- |
| {{SpecName("CSS Logical Properties", "#propdef-min-block-size", "min-block-size")}} | {{Spec2("CSS Logical Properties")}} | Definición inicial. |

## Compatibilidad en navegadores

{{Compat("css.properties.min-block-size")}}

## Mira también

- Las propiedades físicas mapeadas: {{cssxref("min-width")}} y {{cssxref("min-height")}}
- {{cssxref("writing-mode")}}
