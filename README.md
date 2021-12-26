# Custom select nativo (experimental)

De momento no está disponible, sólo se puede probar usando Canary (Edge o Chrome) y habilitando los flags experimentales:

<ul class="unordered-list">
  <li>edge://flags/#enable-experimental-web-platform-features</li>
  <li>chrome://flags/#enable-experimental-web-platform-features</li>
</ul>

Ojalá algún día llegue a todos los navegadores, parece mentira que para las etiquetas <code>&lt;select&gt;</code> no pasara el tiempo, siguen sin poder customizarse sin ningún <code>hack</code> mediante javascript

Se puede obtener más información en el siguiente enlace: <a href="https://open-ui.org/" target="_blank" rel="noopener">https://open-ui.org/</a>

## Etiquetas de custom select nativo

Mirando el código, se puede observar que aparecen dos nuevas etiquetas:

<ul class="unordered-list">
  <li>&lt;selectmenu&gt;: etiqueta contenedora de todo</li>
  <li>&lt;popup&gt;: etiquetas contenedoras de los &lt;option&gt;</li>
</ul>

## Atributos de custom select nativo

Aparecen nuevos atributos relacionados con la activación del selector desplegable y de la opción seleccionada

```html
<div slot="button" behavior="button">
  <button behavior="selected-value"></button>
</div>
```

```html
<popup slot="listbox" behavior="listbox">
  <option>Item</option>
</popup>
```

En este <a href="https://codepen.io/ivan_albizu/pen/YzrEoXO" target="_blank" rel="noopener">PEN</a> puede verse el ejemplo, pero si no estás usando Chrome o Edge Canary con las flags experimentales habilitadas no podrás verlo
