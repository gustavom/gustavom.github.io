---
layout: post
title:  "Terminal: Comandos básicos"
date:   2017-05-31 17:10:41 -0300
categories: terminal linux unix
---

Atualmente, saber utilizar o terminal é quase um requisito básico para qualquer desenvolvedor. Digo quase porque não precisa ser um ninja do teclado, mas saber comandos para navegar entre pastas, arquivos, rodar programas é importante saber.

Assim, fiz uma listinha, que com certeza alguns vão falar que falta algo, mas pode ajudar você no dia a dia.


Os comandos abaixo são focados em linux/unix, o windows compartilha poucos ou quase nenhum, mas eu deixei comentado os que eu achei:


{% highlight shell %}
cd /pasta/
// Navega pela pasta indicada.
{% endhighlight %}

{% highlight shell %}
cd .. 
//win: cd..
// Navega para um nível anterior da pasta.
{% endhighlight %}


{% highlight shell %}
mkdir nome da pasta
// Cria uma pasta.
{% endhighlight %}


As opções "-opção", modificam o comportamento do comando (o terminal do windows não possui opções, pelo que sei).

{% highlight shell %}
ls -a 
// lista todo o conteúdo do diretório, incluindo arquivos e pastas ocultas.
{% endhighlight %}

{% highlight shell %}
ls -l 
// lista todo o conteúdo com informações sobre o arquivo.
{% endhighlight %}

{% highlight shell %}
ls -t 
// ordena os arquivos e pastas de acordo com a data de modificação.
{% endhighlight %}

As opções podem ser usadas juntas, para personalizar a exibição de acordo com o que precisa:

{% highlight shell %}
ls -alt
// opções foram concatenadas:
// - 'a' para mostrar todo o conteúdo da pasta
// - 'l' para mostrar todas as informações dos arquivos e pastas
// = 't' para ordernar por data de modificação
{% endhighlight %}

Pelo terminal, você também pode copiar, mover, remover e renomear arquivos e pastas:

{% highlight shell %}
cp 
// copia o arquivo para o local indicado
{% endhighlight %}

{% highlight shell %}
mv 
// move arquivos e renomeia
{% endhighlight %}

{% highlight shell %}
rm 
// deleta arquivos e pastas
{% endhighlight %}

{% highlight shell %}
rm -r 
// remove a pasta e tudo que esta dentro dela.
{% endhighlight %}

{% highlight shell %}
touch arquivo.txt
// Cria um arquivo.
{% endhighlight %}

{% highlight shell %}
echo "Hello" > arquivo.txt
// vai inserir o conteúdo "Hello" no arquivo arquivo.txt.
{% endhighlight %}

{% highlight shell %}
cat arquivo.txt
// o comando 'cat' mostra o conteúdo do arquivo no terminal.
{% endhighlight %}


{% highlight shell %}
cat arquivo.txt > arquivo2.txt
// passa o conteúdo do primeiro arquivo para o segundo, sobreescrevendo.
{% endhighlight %}

{% highlight shell %}
cat arquivo.txt >> arquivo2.txt
// passa o conteudo do primeiro arquivo para o segundo, mas mantém o conteúdo do arquivo novo.
{% endhighlight %}

{% highlight shell %}
cat arquivo.txt | wc
// mostra no console, sobre o arquivo, respectivamente:
// linhas
// palavras
// caracteres
{% endhighlight %}

{% highlight shell %}
sort arquivo.txt
// mostra no console o conteúdo do arquivo em ordem alfabética
{% endhighlight %}


{% highlight shell %}
uniq arquivo.txt
// mostra no console o conteúdo do arquivo, mas sem mostrar conteúdo repetido.
{% endhighlight %}

{% highlight shell %}
sort arquivo.txt | uniq
// mostra no console o conteúdo do arquivo, em ordem alfabética mas sem mostrar conteúdo repetido.
{% endhighlight %}


{% highlight shell %}
grep filtro arquivo.txt
// O comando 'grep'funciona como filtro de palavras.
// Ex.: grep Mount mountains.txt
// vai retornar as linhas que contém "Mount" no texto.
{% endhighlight %}

{% highlight shell %}
grep -i filtro arquivo.txt
// torna o comando 'grep' 'case insensitive'.
{% endhighlight %}