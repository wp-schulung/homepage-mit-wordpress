---

---

{#kapitel1} 

# Markua and Leanpub (Kapitel 1)

[The Markua Manual by Leanpub](https://leanpub.com/markua/read)

[Markua Website](http://markua.com/)

[The Leanpub Manual](https://leanpub.com/manual/read)



## Markup

Headings

# Überschrift / Heading 1: `# `

## Überschrift / Heading 2: `## `

### Überschrift / Heading 3:`### `

####  Überschrift / Heading 4: `#### `

##### Überschrift / Heading 5: `##### `

###### Überschrift / Heading 6: `###### `



## Verweise und Links

[Linktext](http://#) `[Linktext](url)`

Interner Link zur [Kapitelüberschrift 2](#kapitel2) (vergl. [http://help.leanpub.com](http://help.leanpub.com/author-help/crosslinks-to-chapter-headings-arent-working-in-my-markua-book-what-should-i-be-doing))

(Die Kapitelüberschriften müssen ausgezeichnet werden: `{#kapitel}` am besten direkt vor der Kapitelüberschrift)

{#kapitel2}

Fussnoten werden mit eckigen Klammern und einem "caret" ausgezeichnet. Hinter dem Caret erscheint die ID der Fussnote, die später im Text identisch jedoch zusätzlich mit einem Doppelpunkt am Ende gefolgt von der Erklärung ausgegeben wird.

```
This has a footnote[^thenote].
```

Then, you define the footnote later in the document, using the same  square brackets, caret and tag, followed by a colon, a space and the  footnote definition:

```
[^thenote]: This is the footnote content.
```



## Bilder

[Leanpub Help Center](http://help.leanpub.com/?q=optimal+image+size)

Die maximale Bildergrösse ist abhängig vom Buchformat. Vergl.: [Settings / Image Sizing Help](https://leanpub.com/homepage-mit-wordpress/image_sizing_help)

### Für Bilder im Buch:

- ​         **72 PPI** image: **451** pixels wide x  **698** pixels high.
- ​         **150 PPI** image:  **940** pixels wide x  **1454** pixels high.
- ​         **300 PPI** image:  **1881** pixels wide x  **2907** pixels high.

### Für das Coverbild

- ​         **150 PPI** image: **1240** pixels wide x **1754** pixels high.
- ​         **300 PPI** image: **2481** pixels wide x **3507** pixels high.

ansonsten funktionieren Bilder fast wie Links:

`![Marmalade and Tangerine](resources/marm-and-tangie.jpg)`

![Marmalade and Tangerine](resources/marm-and-tangie.jpg)

standardmässig sind sie zentriert.

Folgende Attribute sind möglich (bzw. werden in diesem Buch genutzt. Vergl. [The Markua Manual > Images](https://leanpub.com/markua/read#images))

align: left | right | middle

alt: 

width / height: percentage 1%-100%, use golden ratio: 72:28



```markdown
{alt: "Alternativer Alternativ-Text?", align: right, width: 28%}
![Marmalade and Tangerine](resources/marm-and-tangie.jpg
```



{alt: "Alternativer Alternativ-Text?", align: left, width: 28%}
![Marmalade and Tangerine](resources/marm-and-tangie.jpg)

## Zitate

Quotes beginnen mit > und einem Leerschlag:

> Dies ist ein Zitat.

Für längere Zitate geht es auch mit

```markdown
{blockquote} … {/blockquote}
```

# Kapitel 2

(dient dem Zeigen von Querverlinkung)

zurück zu [Kapitel1](#kapitel1)