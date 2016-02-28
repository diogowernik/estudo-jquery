### Intro

#### Encontrar e Modificar simples

1) Encontrar

    $("h2").text();
    $(".navbar").text();

2) Modificar

    $("h2").text("yoga.brasilia.io");

3) Apenas iniciar o jquery quando a pagina e funções já estiverem carregadas

    jQuery(document).ready(function(){
    
    <code>
    
    });
    

4) Mais...

    $("p");
    $("#container");
    $(".articles");

5) Seletor abaixo

    $("#navbar-right li");
    $("#navbar-right li:first");
    $("#navbar-right li:last");

Pares e impares (inicia no [0])

    $("#navbar-right li:odd");
    $("#navbar-right li:even");

6) selecionar filhos diretos x selecionar todos filhos e netos

Todos

    $("#navbar-right li");

Apenas filhos diretos

    $("#navbar-right > li");

7) Selecionar elemento multiplos

    $("#navbar-right, .social");