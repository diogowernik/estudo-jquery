### Alguns Métodos

####Traversing

find()

    $(".navbar-right li");

    $(".navbar-right").find("li");

first() & last() 

    $("li:first");

    $("li").first();
    $("li").last();

next()

    $("li").first().next();

parent()

    $("li").first().parent();

children()

Apenas filhos diretos

    $(".navbar-right > li");

    $(".navbar-right").children("li");
    





