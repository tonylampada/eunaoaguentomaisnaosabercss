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

/* Todos os <p>'s que forem descendentes de <span>'s */
p span {
	...
}

```

### [Classes e ids](http://tonylampada.github.io/eunaoaguentomaisnaosabercss/seletores/classes_e_ids.html)

* Id's devem ser únicos
* Dá pra combinar classes diferentes no mesmo elemento.

```css
/* seleciona quem tiver class="main-header" */
.main-header {
	...
}

/* Quem tiver id="main-content" */
#main-content {
	...
}

/* Os <p>'s que forem descendentes de alguem com id="main-content" */
#main-content p {
	...
}

```

### [Tudo em família](http://tonylampada.github.io/eunaoaguentomaisnaosabercss/seletores/estruturais.html)

* > Filhos diretos
* + Irmãos adjacentes
* ~ Quaisquer irmãos

```css
/* Todos os links que forem filhos diretos de class="main" */
.main > a {
	...
}

/* Todos os <p>'s que forem irmãos de <h2>'s */
h2 ~ p {
	...
}

/* Todos os <p>'s que forem adjacentes a <h2>'s */
h2 + p {
	...
}


```

* [Direct child](http://tonylampada.github.io/eunaoaguentomaisnaosabercss/seletores/directhild.html)
* [Sibling](http://tonylampada.github.io/eunaoaguentomaisnaosabercss/seletores/sibling.html)
* [Pseudo-classes](http://tonylampada.github.io/eunaoaguentomaisnaosabercss/seletores/pseudoclasses.html)
* [first-child, last-child, nth-child](http://tonylampada.github.io/eunaoaguentomaisnaosabercss/seletores/nthchild.html)
* [Pseudo-elements / generated content](http://tonylampada.github.io/eunaoaguentomaisnaosabercss/seletores/pseudoelements.html)

# O Box Model



# Flexbox

# Media Queries