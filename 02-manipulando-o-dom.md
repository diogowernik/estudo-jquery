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

### Anexar (append)

append()
prepend()
after()
before()

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