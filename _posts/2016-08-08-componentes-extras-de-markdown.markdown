---
title: Componentes extras de markdown
layout: post
date: '2016-08-08 10:30'
tag:
- markdown
- componentes
- extra
blog: true
star: true
---

## Sumário:

Escolha um item para ver a aplicação no markdown.

#### Especial Elements

- [Evidência](#evidence)
- [Lado a lado](#side-by-side)
- [Star](#star)
- [Linha especial](#especial-breaker)

#### External Elements

- [Gist](#gist)
- [Codepen](#codepen)
- [Slideshare](#slideshare)
- [Videos](#videos)

---

## Evidência {#evidence}

Você pode usar evidências!

<span class="evidence">Parágrafos podem ser escrito como tal. Um parágrafo é um bloco básico de markdown. Um parágrafo é o que o texto vai ser quando não há nenhuma razão para ser outra coisa.</span>

{% highlight html %}
<span class="evidence">Parágrafos podem ser escrito como tal. Um parágrafo é um bloco básico de markdown. Um parágrafo é o que o texto vai ser quando não há nenhuma razão para ser outra coisa.</span>
{% endhighlight %}

---

## Lado a lado {#side-by-side}

Assim como no [Medium](https://medium.com/).

**Imagem** a esquerda e **Texto** a direita:

{% highlight html %}
<div class="side-by-side">
    <div class="toleft">
        <img class="image" src="{{ site.url }}/{{ site.picture }}" alt="Alt Text">
        <figcaption class="caption">João Vinicius</figcaption>
    </div>

    <div class="toright">
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>
</div>
{% endhighlight %}

<div class="side-by-side">
    <div class="toleft">
        <img class="image" src="{{ site.url }}/{{ site.picture }}" alt="Alt Text">
        <figcaption class="caption">João Vinicius</figcaption>
    </div>

    <div class="toright">
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>
</div>

**Texto** a esquerda e **Imagem** a direita:

{% highlight html %}
<div class="side-by-side">
    <div class="toleft">
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>

    <div class="toright">
        <img class="image" src="{{ site.url }}/{{ site.picture }}" alt="Alt Text">
        <figcaption class="caption">João Vinicius</figcaption>
    </div>
</div>
{% endhighlight %}

<div class="side-by-side">
    <div class="toleft">
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>

    <div class="toright">
        <img class="image" src="{{ site.url }}/{{ site.picture }}" alt="Alt Text">
        <figcaption class="caption">João Vinicius</figcaption>
    </div>
</div>

---

## Star {#star}

Você pode evidenciar um post. É só adicionar a tag ao arquivo markdown.

{% highlight raw %}
star: true
{% endhighlight %}

---

## Linha especial {#especial-breaker}

Você pode adicionar um *hr* especial ao seu texto.

{% highlight html %}
<div class="breaker"></div>
{% endhighlight %}

<div class="breaker"></div>

---

## Gist {#gist}

Você pode adicionar Gists do github.

{% highlight raw %}
{ % gist sergiokopplin/91ff4220480727b47224245ee2e9c291 % }
{% endhighlight %}

{% gist sergiokopplin/91ff4220480727b47224245ee2e9c291 %}

---

## Codepen {#codepen}

Você pode adicionar Pens do Codepen.

{% highlight html %}
<p data-height="268" data-theme-id="0" data-slug-hash="gfdDu" data-default-tab="result" data-user="chriscoyier" class='codepen'>
    See the Pen <a href='http://codepen.io/chriscoyier/pen/gfdDu/'>Crappy Recreation of the Book Cover of *The Flame Alphabet*</a> by Chris Coyier (<a href='http://codepen.io/chriscoyier'>@chriscoyier</a>) on <a href='http://codepen.io'>CodePen</a>.
</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>
{% endhighlight %}

<p data-height="268" data-theme-id="0" data-slug-hash="gfdDu" data-default-tab="result" data-user="chriscoyier" class='codepen'>See the Pen <a href='http://codepen.io/chriscoyier/pen/gfdDu/'>Crappy Recreation of the Book Cover of *The Flame Alphabet*</a> by Chris Coyier (<a href='http://codepen.io/chriscoyier'>@chriscoyier</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

---

## Slideshare {#slideshare}

Você pode adicionar suas apresentações aqui!

{% highlight html %}
<iframe src="//www.slideshare.net/slideshow/embed_code/key/hqDhSJoWkrHe7l" width="560" height="310" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe>
{% endhighlight %}

<iframe src="//www.slideshare.net/slideshow/embed_code/key/hqDhSJoWkrHe7l" width="560" height="310" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe>

---

## Videos {#videos}

Você deseja alguns videos? Youtube, Vimeo ou Vevo? Copie o código de incorporação e cole no seu post!

**Exemplo**

{% highlight html %}
<iframe width="560" height="310" src="https://www.youtube.com/embed/r7XhWUDj-Ts" frameborder="0" allowfullscreen></iframe>
{% endhighlight %}

<iframe width="560" height="310" src="https://www.youtube.com/embed/r7XhWUDj-Ts" frameborder="0" allowfullscreen></iframe>

[1]: http://daringfireball.net/projects/markdown/
[2]: http://www.fileformat.info/info/unicode/char/2163/index.htm
[3]: http://www.markitdown.net/
[4]: http://daringfireball.net/projects/markdown/basics
[5]: http://daringfireball.net/projects/markdown/syntax
[6]: http://kune.fr/wp-content/uploads/2013/10/ghost-blog.jpg

Tradução do [post](https://koppl.in/indigo/markdown-extra-components/){: target="_blank" }.
