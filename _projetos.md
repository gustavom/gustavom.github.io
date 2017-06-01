---
layout: page
title: Projetos
permalink: /projetos/
---

Compartilho aqui com você alguns projetos que participei:

{% if site.projetos.size == 0 %}
    <!--<h2>No post found</h2>-->
{% else %}
{% for projetos in site.projetos %}
      <div class="list-item">
        <h2 class="list-post-title">
          <a href="{{ site.baseurl }}{{ projetos.url }}">{{ projetos.title }}</a>
        </h2>
        <div class="list-post-date">
          <time>{{ projetos.date | date_to_string }}</time>
        </div>
      </div>
    {% endfor %}
 {% endif %}



<h2 class="projeto-title">PLATAFORMA DE E-COMMERCE HIGHCOMMERCE</h2>

Plataforma de e-commerce própria da empresa HighCommerce. Projeto que trabalhei nos últimos 4 anos e meio, em que participo desde o início do desenvolvimento.

Pensado e criado para atender a diversos mercados, diversos tamanhos de empresa, do pequeno ao grande porte.

Grandes possibilidades de customização do layout da loja, afim de alinhar o visual da loja com a identidade da marca do cliente e como ele pretende se comunicar e atender o seu público alvo.

Fui responsável direto pela arquitetura e desenvolvimento front-end.

[![Plataforma HighCommerce](/assets/images/highcommerce-plataforma.jpg)](http://www.highcommerce.com.br/){:target="_blank"}   

<h2 class="projeto-title">KREATIVE CATÁLOGO</h2>

Produto desenvolvido para suprir rápidamente a necessidade de clientes que buscam um projeto moderno, com layout customizável, design responsivo para diversos dispositivos, tanto para um site institucional, tanto para um catálogo online.

Fui responsável direto pela arquitetura e desenvolvimento front-end.

[![Kreative Catálogo](/assets/images/kreative-catalogo.jpg)](http://www.kreative.net.br/catalogo/){:target="_blank"}

<h2 class="projeto-title">PUC-SP | Ex-Alunos em Destaque</h2>

Projeto interno da PUC-SP, para divulgar ex-alunos da instituição que possuem destaque na sociedade, assim, podem compartilhar suas histórias e experiências.

[![Ex-alunos em Destaque PUC-SP](/assets/images/puc-ex-alunos-destaque.jpg)](http://www.pucsp.br/destaque/){:target="_blank"}