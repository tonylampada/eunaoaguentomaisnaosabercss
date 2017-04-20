eunaoaguentomaisnaosabercss
===========================

Condensação dos meus aprendizados sobre CSS

# Links:
(valeu aih galera)

* [Chegou a hora de estudar CSS(facebook)](https://www.facebook.com/groups/desenvolvimentoweb/permalink/676490642409378/)
* [Media queries (w3c)](http://www.w3.org/TR/css3-mediaqueries/)
* [Responsive Web Design for Beginners (tutsplus.com)](https://tutsplus.com/course/responsive-web-design-for-beginners/)
* [box-sizing: border-box FTW (blog Paul Irish)](http://www.paulirish.com/2012/box-sizing-border-box-ftw/)
* [CSS snippets](http://css-tricks.com/snippets/)
* [Grid - guide to responsive design](http://www.adamkaplan.me/grid/)
* [scss toolkit](https://github.com/davidrapson/scss-toolkit)
* [html5boilerplate](http://html5boilerplate.com/)
* [Normalize.css](https://github.com/necolas/normalize.css/)
* [960.gs](http://960.gs/)
* [Eric Meyer CSS reset](http://meyerweb.com/eric/tools/css/reset/)
* [Front end style guides](http://24ways.org/2011/front-end-style-guides/)
* [KSS (gerador de documentação de CSS)](http://warpspire.com/posts/kss/)
* [html5rocks](http://www.html5rocks.com/)
* [A begginners guide to wireframing](http://webdesign.tutsplus.com/articles/a-beginners-guide-to-wireframing--webdesign-7399)

# 1. Seletores:

### [Element](http://tonylampada.github.io/eunaoaguentomaisnaosabercss/seletores/type.html)

```css
/* Isso seleciona a porra toda */
* {
	...
}

/* Todos os <h1>'s */
h1 {
	...
}

/* Todos os <span>'s descendentes de <p>'s */
p span {
	...
}

```

### [Classes e ids](http://tonylampada.github.io/eunaoaguentomaisnaosabercss/seletores/classes_e_ids.html)

* .classe
* #id
* Id's devem ser únicos
* Dá pra combinar classes diferentes no mesmo elemento.

### [Tudo em família](http://tonylampada.github.io/eunaoaguentomaisnaosabercss/seletores/estruturais.html)

* `>` Filhos diretos
* `+` Irmão seguinte
* `~` Quaisquer irmãos subsequentes
* `+` e ~ só pegam os irmão que aparecem DEPOIS do elemento

### [Attribute](http://tonylampada.github.io/eunaoaguentomaisnaosabercss/seletores/attribute.html)

* [atributo]
* [atributo="valor"]
* [atributo^="startswith"]
* [atributo$="endswith"]
* [atributo*="contains"]

### [Pseudo-classes](http://tonylampada.github.io/eunaoaguentomaisnaosabercss/seletores/pseudoclasses.html)
(Muito foda isso...)

* a:link - links nao visitados
* a:visited - links ja visitados
* :target - o div com id="ancora" se o cara caiu no link que termina com #ancora
* :hover - mouse em cima
* :active - mouse clicado em cima
* :focus - links ou inputs que estão com foco
* :enabled - inputs/botoes habilitados
* :disabled - inputs/botoes desabilitados
* :checked - checkbox/radio selecionados
* :empty - só seleciona se tiver vazio
* :not(<seletor>) - só seleciona quem não obedecer a condição do seletor
* :first-child - só o primeiro filho
* :last-child - só o último filho
* :only-child - só se for filho único
* :nth-child(even) - só os filhos pares
* :nth-child(odd) - só os filhos ímpares
* :nth-child(3n+2) - 2o, 5o, 8o...
* div:nth-of-type(3n+2) - 2o, 5o, 8o... mas só os divs
* div:only-of-type - só se for o único div filho

### [Pseudo-elements / generated content](http://tonylampada.github.io/eunaoaguentomaisnaosabercss/seletores/pseudoelements.html)

* Pseudoelementos podem vir com :: ou com : (prefira :: por clareza)
* ::first-line - seleciona só a primeira linha do texto dentro do elemento
* ::first-letter - seleciona só a primeira LETRA do texto dentro do elemento
* ::before - ADICIONA um pseudoelemento como primeiro filho do elemento.
* ::after - ADICIONA um pseudoelemento como último filho do elemento.
* ::before e ::after tem que ter um atributo content (que seja no minimo uma string vazia)
* O atributo content pode ser:
** Uma string
** Uma chamada da funcão url
** Uma chamada da função attr (que pega o valor de um atributo do elemento)
* Dá pra criar formas interessantes (círculos, elipses, etc) com before e after

```css
/* Adiciona um ícone de telefone depois */
.phone::after {
	content: "\2706";
}

/* Adiciona um ícone de pdf antes */
.pdf::before {
	content: url(../img/pdf.gif);
	margin: 0 8px;
}

/* Adiciona a url do link depois */
.pdf::after {
	content: attr(href);
	padding-left: 10px;
	color: red;
}
```

# O Box Model

# Flexbox

# Media Queries
