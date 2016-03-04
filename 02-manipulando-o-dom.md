### 02 - Manipulando o DOM

Função do Jquery quando o documento estiver pronto!

```javascript
$(document).ready(function() {




});
```

Adicionando tags html

```javascript
var name = $('<p>João</p>');
```

#### Ações

Exemplo:

```javascript
<li class="card">
    <h2></h2>
    <button>
</li>
```

**before()**

```javascript
var name = $('<p>João</p>');
$('.card').before(name);

<p>João<p>
<li class="card">
    <h2></h2>
    <button>
</li>
```

**after()**

```javascript
var name = $('<p>João</p>');
$('.card').before(name);

<li class="card">
    <h2></h2>
    <button>
</li>
<p>João<p>
```

**prepend()**

```javascript
var name = $('<p>João</p>');
$('.card').prepend(name);

<li class="card">
    <p>João<p>
    <h2></h2>
    <button>
</li>
```

**append()**

```javascript
var name = $('<p>João</p>');
$('.card').append(name);

<li class="card">
    <h2></h2>
    <button>
    <p>João<p>
</li>
```

Is possible also to use like:

**appendTo()**

```javascript
name.appendTo($('.card'));
```

**insertAfter()**

```javascript
name.insertAfter($('.card'));
```

**prependTo()**

```javascript
name.prependTo($('.card'));
```

**insertBefore()**

```javascript
name.prependTo($('.card'));
```

#### Remove

**remove()**

```javascript
var name = $('<p>João</p>');
$('.card').append(name);

$('button').remove();

<li class="card">
    <h2></h2>
    
    <p>João<p>
</li>
```


#### Algo acontece quando o button é clicado

```javascript
$('button').on('click', function() {



});
```

Exemplo:

```javascript
$('button').on('click', function() {

    var name = $('<p>João</p>');
    $('.card').append(name);
    $('button').remove();

});
```

Quando clicar no botão... acontece:

variavel criada: **João**

nome adicionado ao **.card**

**button** removido


#### Usando o (this)

Fica:


```javascript
$('button').on('click', function() {

    var name = $('<p>João</p>');
    $('this').closest(.card).append(name);
    $('this').remove();

});
```

Traduzindo:

Cria a variável **João**

Adiciona a variável no **card** pai do **button**, 

ou seja o (this) aqui é o **button**.

remove o **button**
