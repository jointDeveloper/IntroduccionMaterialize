![jointDeveloper](https://raw.githubusercontent.com/jointDeveloper/Aprendizaje-Web/gh-pages/IMG/robot-logo.png)

# Taller Práctico Materialize

* Vamos a la pagina de [Materialize](http://materializecss.com/).

* Damos clic en GET STARTED.

![jointDeveloper](https://raw.githubusercontent.com/jointDeveloper/IntroduccionMaterialize/master/images/img1.png)

* Damos clic en Materialize.

![jointDeveloper](https://raw.githubusercontent.com/jointDeveloper/IntroduccionMaterialize/master/images/img2.png)

* Descomprimimos la carpeta descargada.
* Creamos un archivo ***index.html*** con la siguiente información.
```html
<!DOCTYPE html>
<html>
  <head>
  <!--Import Google Icon Font-->
    <link href="http://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
    <!--Import materialize.css-->
    <link type="text/css" rel="stylesheet" href="css/materialize.min.css"  media="screen,projection"/>

    <!--Let browser know website is optimized for mobile-->
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  </head>

  <body>
  <!--Import jQuery before materialize.js-->
    <script type="text/javascript" src="https://code.jquery.com/jquery-2.1.1.min.js"></script>
    <script type="text/javascript" src="js/materialize.min.js"></script>
  </body>
</html>
```

* Agregamos un titulo a nuestra pagina.
```html
<!DOCTYPE html>
<html>
  <head>
  <!--Import Google Icon Font-->
    ...
    <title>jointDeveloper Shop</title>
  </head>
```
## Inicio de nuestra página
### Navbar
* Vamos a la pagina de [Materialize](http://materializecss.com/) y damos clic en Components y luego en Navbar.

![jointDeveloper](https://raw.githubusercontent.com/jointDeveloper/IntroduccionMaterialize/master/images/img3.png)

* Seleccionamos el Navbar que más nos guste y copiamos el código. Para nuestro caso seleccionamos este:
  ```html
  <nav>
    <div class="nav-wrapper">
      <a href="#" class="brand-logo">Logo</a>
      <ul id="nav-mobile" class="right hide-on-med-and-down">
        <li><a href="sass.html">Sass</a></li>
        <li><a href="badges.html">Components</a></li>
        <li><a href="collapsible.html">JavaScript</a></li>
      </ul>
    </div>
  </nav>
  ```
* Escribimos el script de inicialización.
```javascript
<script>
     $(document).ready(function() {
        $('select').material_select();
        $(".button-collapse").sideNav();
    });
</script>
```
* Vamos a agregar la propiedad ***navbar-fixed***.
  ```html
  <div class="navbar-fixed">
    <nav>
      <div class="nav-wrapper">
        ...
    </nav>
  </div>  
  ```
### Icons
* Vamos a la pagina de [Materialize](http://materializecss.com/) y damos clic en Components y luego en Icons.

![jointDeveloper](https://raw.githubusercontent.com/jointDeveloper/IntroduccionMaterialize/master/images/img4.png)

* Copiamos la linea de iconos y seleccionamos el icono que mas nos guste.
  ```html
  <div class="navbar-fixed">
    <nav>
      <div class="nav-wrapper" >
        <a href="#" class="brand-logo center"><i class="large material-icons">shopping_cart</i></a>
        ...
      </div>
    </nav>
  </div>
  ```
## Titulo de nuestra pagina
* Vamos a Escribir el Titulo de nuestra página.
  * HTML
    ```html
    <div class="fondo">
      <div class="row container" id="index">
        <h1 class="center">jointDeveloper Shop</h1>
      </div>
    </div>
    ```
  * CSS  
    ```css
    .fondo {
      background-image: url(../img/fondo.jpg);
    }
    ```

## Contenido de la página
* Vamos a llenar el contenido de nuestra página.
  ```html
  <div class="row container" id="info">
    <div class="col s8">
      <p>
        ...
      </p>
    </div>
    <div class="col s4">
      <img src="img/venta.jpg" alt="" />
    </div>
  </div>  
  ```
## Nuestros Productos
* Para darle un titulo a esta sección hacemos lo siguiente:
```html
<div class="grey lighten-3">
 <div class="row container" id="productos">
   </br>
   <h2 class="center">Nuestros Productos</h2>
   </br>
   <div class="col s4">
     ...
   </div>
 </div>
</div>    
```         
### Cards    
* Vamos a la pagina de [Materialize](http://materializecss.com/) y damos clic en Components y luego en Cards.

![jointDeveloper](https://raw.githubusercontent.com/jointDeveloper/IntroduccionMaterialize/master/images/img5.png)

* Seleccionamos la Card que más nos guste y la pegamos en nuestro código. Para nuestro caso seleccionamos este:
```html
<div class="card">
   <div class="card-image waves-effect waves-block waves-light">
     <img class="activator" src="images/office.jpg">
   </div>
   <div class="card-content">
     <span class="card-title activator grey-text text-darken-4">Card Title<i class="material-icons right">more_vert</i></span>
     <p><a href="#">This is a link</a></p>
   </div>
   <div class="card-reveal">
     <span class="card-title grey-text text-darken-4">Card Title<i class="material-icons right">close</i></span>
     <p>Here is some more information about this product that is only revealed once clicked on.</p>
   </div>
 </div>
 ```
## Contactanos
* Le damos un titulo:
```html
<div class="row container" id="contacto">
  <h2 class="center">Contactanos</h2>
</div>
```
### Forms
* Vamos a la pagina de [Materialize](http://materializecss.com/) y damos clic en Components y luego en Forms.

![jointDeveloper](https://raw.githubusercontent.com/jointDeveloper/IntroduccionMaterialize/master/images/img6.png)

* Copiamos el código del input field > icon prefixes
```html
<div class="row">
  <form class="col s12">
    <div class="row">
      <div class="input-field col s6">
        <i class="material-icons prefix">account_circle</i>
        <input id="icon_prefix" type="text" class="validate">
        <label for="icon_prefix">First Name</label>
      </div>
      <div class="input-field col s6">
        <i class="material-icons prefix">phone</i>
        <input id="icon_telephone" type="tel" class="validate">
        <label for="icon_telephone">Telephone</label>
      </div>
    </div>
  </form>
</div>
```
* Modificamos para agregar un email:
```html
 <div class="input-field col s6">
   <i class="material-icons prefix">email</i>
   <input id="email" type="email" class="validate">
   <label for="email">Email</label>
 </div>
```
* Copiamos el codigo de Textarea > Icon prefixes:
```html
<div class="row">
   <form class="col s12">
     <div class="row">
       <div class="input-field col s6">
         <i class="material-icons prefix">mode_edit</i>
         <textarea id="icon_prefix2" class="materialize-textarea"></textarea>
         <label for="icon_prefix2">First Name</label>
       </div>
     </div>
   </form>
 </div>
```
### Buttons
* Vamos a la pagina de [Materialize](http://materializecss.com/) y damos clic en Components y luego en Buttons.

![jointDeveloper](https://raw.githubusercontent.com/jointDeveloper/IntroduccionMaterialize/master/images/img7.png)

* Seleccionamos el boton que mas nos guste, en nuestro caso usaremos un ***Submit Button***:
```html
<button class="btn waves-effect waves-light" type="submit" name="action">Submit
  <i class="material-icons right">send</i>
</button>
```     
## Footer
* Vamos a la pagina de [Materialize](http://materializecss.com/) y damos clic en Components y luego en Footer.

![jointDeveloper](https://raw.githubusercontent.com/jointDeveloper/IntroduccionMaterialize/master/images/img8.png)  

* Copiamos el código y lo editamos a nuestro gusto:
```html
<footer class="page-footer">
  <div class="container">
    <div class="row">
      <div class="col l6 s12">
        <h5 class="white-text">Footer Content</h5>
        <p class="grey-text text-lighten-4">You can use rows and columns here to organize your footer content.</p>
      </div>
      <div class="col l4 offset-l2 s12">
        <h5 class="white-text">Links</h5>
        <ul>
          <li><a class="grey-text text-lighten-3" href="#!">Link 1</a></li>
          <li><a class="grey-text text-lighten-3" href="#!">Link 2</a></li>
          <li><a class="grey-text text-lighten-3" href="#!">Link 3</a></li>
          <li><a class="grey-text text-lighten-3" href="#!">Link 4</a></li>
        </ul>
      </div>
    </div>
  </div>
  <div class="footer-copyright">
    <div class="container">
    © 2014 Copyright Text
    <a class="grey-text text-lighten-4 right" href="#!">More Links</a>
    </div>
  </div>
</footer>
```  
### CSS            
* Algunas clases importantes en el CSS:
```css
img {
  width: 80%;
  height: 70%;
}
h1 {
  font-family: 'Linden Hill', serif;
  font-size: 5em;
  font-weight: bold;
}
#index, #info, #productos, #contacto{
  padding-top: 60px;
}
.grey {
  background-color: #eeeeee;
}
```
