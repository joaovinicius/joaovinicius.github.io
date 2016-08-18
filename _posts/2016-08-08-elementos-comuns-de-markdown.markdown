---
title: Elementos comuns de markdown
layout: post
date: '2016-08-08 09:30'
tag:
- markdown
- elementos
blog: true
star: true
---

## Sumário:

Você pode escolher um item para ver como markdown é aplicado.

### Elementos básicos

- [Formatação básica](#basic-formatting)
- [Cabeçalhos](#headings)
- [Listas](#lists)
- [Modificadores de parágrafos](#paragraph-modifiers)
- [Urls](#urls)
- [Linhas horizontais](#horizontal-rule)
- [Imagens](#images)
- [Códigos](#code)

---

## Formatação básica {#basic-formatting}

Esta nota **demonstra** um pouco do que [Markdown][1] é *capaz de fazer*.

E é assim que se faz.

{% highlight html %}
Esta nota **demonstra** um pouco do que [Markdown][some/link] é *capaz de fazer*.
{% endhighlight %}

---

## Cabeçalhos {#headings}

Existem seis níveis de cabeçalhos. Eles correspondem aos seis níveis de cabeçalhos HTML. Você provavelmente já notou eles na página. Para cada nível baixo usa mais um caractere hash. Mas nós estamos usando apenas 4 deles.

# Cabeçalhos podem ser pequenos

## Cabeçalhos podem ser pequenos

### Cabeçalhos podem ser pequenos

#### Cabeçalhos podem ser pequenos

{% highlight raw %}
# Cabeçalho
## Cabeçalho
### Cabeçalho
#### Cabeçalho
{% endhighlight %}

---

## Listas {#lists}

### Listas ordenadas

1. Item 1
2. Segundo item
3. Número 3

{% highlight raw %}
1. Item 1
2. Segundo item
3. Número 3
{% endhighlight %}

### Listas desordenadas

* Um item
* Outro item
* Mais um item
* E podem haver mais...

{% highlight raw %}
* Um item
* Outro item
* Mais um item
* E podem haver mais...
{% endhighlight %}

---

## Modificadores de parágrafos {#paragraph-modifiers}

### Citação

> Aqui está uma citação. Isso deve ser auto-explicativo. As citações são recuadas automaticamente quando usadas.

{% highlight raw %}
> Aqui está uma citação. Isso deve ser auto-explicativo.
{% endhighlight raw %}

---

## URLs

As URLs podem ser feitas de um punhado de maneiras:

* Um link para [Mark It Down][3].
* Outro link para [Mark It Down](http://markitdown.net/)
* As vezes você quer só uma URL como <http://markitdown.net/>.

{% highlight raw %}
* Um link para [Mark It Down][3].
* Outro link para [Mark It Down](http://markitdown.net/)
* As vezes você quer só uma URL como <http://markitdown.net/>.
{% endhighlight %}

---

## Linhas horizontais {#horizontal-rule}

Uma regra horizontal é uma linha que atravessa o meio da página.
Às vezes é útil para separar as coisas.

{% highlight raw %}
---
{% endhighlight %}

---

## Imagens {#images}

Markdown também podem conter imagens. Vou precisar de acrescentar algo aqui algum dia.

{% highlight raw %}
![Markdowm Image][/image/url]
{% endhighlight %}

![Markdowm Image][6]

*Descrição da imagem*?

{% highlight raw %}
![Markdowm Image][/image/url]
<figcaption class="caption">Foto por John Doe</figcaption>
{% endhighlight %}

![Markdowm Image][6]
<figcaption class="caption">Foto por John Doe</figcaption>

*Imagens Grandes*?

{% highlight raw %}
![Markdowm Image][/image/url]{: class="bigger-image" }
{% endhighlight %}

![Markdowm Image][6]{: class="bigger-image" }

---

## Códigos {#code}

Exemplo de HTML:

{% highlight html %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
</head>
<body>
    <h1>Just a test</h1>
</body>
</html>
{% endhighlight %}

Exemplo de CSS:

{% highlight css %}
pre {
    padding: 10px;
    font-size: .8em;
    white-space: pre;
}

pre, table {
    width: 100%;
}

code, pre, tt {
    font-family: Monaco, Consolas, Inconsolata, monospace, sans-serif;
    background: rgba(0,0,0,.05);
}
{% endhighlight %}

Exemplo de JS:

{% highlight js %}
// Sticky Header
$(window).scroll(function() {

    if ($(window).scrollTop() > 900 && !$("body").hasClass('show-menu')) {
        $('#hamburguer__open').fadeOut('fast');
    } else if (!$("body").hasClass('show-menu')) {
        $('#hamburguer__open').fadeIn('fast');
    }

});
{% endhighlight %}

[1]: http://daringfireball.net/projects/markdown/
[2]: http://www.fileformat.info/info/unicode/char/2163/index.htm
[3]: http://www.markitdown.net/
[4]: http://daringfireball.net/projects/markdown/basics
[5]: http://daringfireball.net/projects/markdown/syntax
[6]: http://kune.fr/wp-content/uploads/2013/10/ghost-blog.jpg

Tradução do [post](https://koppl.in/indigo/markdown-common-elements/){: target="_blank" }.
