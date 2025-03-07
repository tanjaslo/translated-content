---
title: border-inline-style
slug: Web/CSS/border-inline-style
tags:
  - CSS
  - Experimental
  - Propriété
  - Propriété logique
  - Reference
translation_of: Web/CSS/border-inline-style
---
{{CSSRef}}{{SeeCompatTable}}

La propriété** `border-inline-style`** permet de définir le style pour la bordure sur les côtés d'un élément qui correspondent à l'axe en ligne. Cette propriété logique correspond à différentes propriétés physiques selon le mode d'écriture, la direction et l'orientation du texte. Autrement dit, cette propriété correspond à {{cssxref("border-top-style")}} et {{cssxref("border-bottom-style")}} ou à {{cssxref("border-left-style")}} et {{cssxref("border-right-style")}} selon les valeurs des propriétés {{cssxref("writing-mode")}}, {{cssxref("direction")}} et {{cssxref("text-orientation")}}.

```css
/* Valeurs de type <'border-style'> */
border-inline-style: dashed;
border-inline-style: dotted;
border-inline-style: groove;
```

Pour les autres côtés, la bordure peut être mise en forme grâce à la propriété {{cssxref("border-block-style")}} qui définit {{cssxref("border-block-start-style")}} et {{cssxref("border-block-end-style")}}.

## Syntaxe

### Valeur

- `<'border-style'>`
  - : Le style de la ligne pour la bordure. Voir {{ cssxref("border-style") }}.

### Syntaxe formelle

{{csssyntax}}

## Exemples

### CSS

```css
div {
  background-color: yellow;
  width: 120px;
  height: 120px;
}

.texteExemple {
  writing-mode: vertical-lr;
  border: 5px solid blue;
  border-inline-style: dashed;
}
```

### HTML

```html
<div>
  <p class="texteExemple">Texte exemple</p>
</div>
```

### Résultat

{{EmbedLiveSample("Exemples", 140, 140)}}

## Spécifications

| Spécification                                                                                                                | État                                             | Commentaires         |
| ---------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------ | -------------------- |
| {{SpecName("CSS Logical Properties", "#propdef-border-inline-style", "border-inline-style")}} | {{Spec2("CSS Logical Properties")}} | Définition initiale. |

{{cssinfo}}

## Compatibilité des navigateurs

{{Compat("css.properties.border-inline-style")}}

## Voir aussi

- Les propriétés physiques qui correspondent à cette propriété logique :

  - {{cssxref("border-top-style")}},
  - {{cssxref("border-right-style")}},
  - {{cssxref("border-bottom-style")}},
  - {{cssxref("border-left-style")}}.

- {{cssxref("writing-mode")}}, {{cssxref("direction")}}, {{cssxref("text-orientation")}}
