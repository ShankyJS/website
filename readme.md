tipos de posiciones
-static = la predeterminada estatica
-absolute = se sale de donde estaba ubicado inicialmente, pierde su espacio y se va a colocar de manera absoluta, Va a ser relativo con el objeto mas cercano que tenga seteado el position relative
-fixed = fijo es un elemento fijo que se queda alli y se queda allí así hagamos scroll
-sticky = es cuando pasas una sección haciendo scroll y se te pega en la parte superior o donde quisieramos

Cuando aplicamos cualquiera de estos position se desbloquean:
z-indez
top bottom left y right y sirven para mover el elemento a donde quisieramos



````

<div class="section">

</div>
<div class="section sticky">
  <p>Hola <span class="mundo">mundo</span>
  <span class="responsive">Responsive Design</span>
  </p>
</div>
<div class="section">

</div>


<div class="section">

</div>
````

````

.section {
  height: 200px;
  background: lightgray;
  margin: 10px 0;
  border: 1px solid red;
/*   position: relative */
}
p {
  font-size: 3em;
  background: red;
  display: inline-block;
  position: relative;
}
p span {
/*   position: fixed; */
/*   right: -200px; */
/*   background: blue; */
/*   right: 0;
  top: 0; */
}
.mundo {
  background: pink;
  z-index: 8;
}
.responsive {
  background: yellow;
  z-index: 7;
}

/* static
realtive
absolute
fixed
sticky */

/* z-index */
/* top right bottom left */
.sticky {
  position: sticky;
  top: 0;
  background: rgba(0,0,0,.5)
}

````