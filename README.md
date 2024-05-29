<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nueva pestaña</title>
    <!--CONEXIÓN CON CSS-->
   <link rel="stylesheet" href="css/main.css"> <!-- Cambiado "main-css" a "main.css" y corregida la ruta -->
</head>
<body>
    <!--ENCABEZADO-->
    <!-- Contiene elementos de encabezado o navegación-->
    <header>
        <!--Pueden haber más elementos en el header-->
        <!-- nav= Aporta la capacidad de navegación-->
        <nav>
            <!-- Lista ordenada-->
            <ul class="nav-right-section">
                <li>
                    <a href="">Gmail</a>
                </li>
                <li>
                    <a href="">Imágenes</a>
                </li>
                <li class="menu">
                    <a href="">  </a>
                </li>
                <li>
                    <a href="" > <img src="https://lh3.google.com/u/0/ogw/AF2bZyidqHfCKK7YVnowW0gv3Oyhji58NlVCOSOnf2sSszsEiA=s32-c-mo" srcset="https://lh3.google.com/u/0/ogw/AF2bZyidqHfCKK7YVnowW0gv3Oyhji58NlVCOSOnf2sSszsEiA=s32-c-mo 1x" alt="Foto de ícono E" class="fotoE" > </a>
                </li>
            </ul>
        </nav>
    </header>
    <main>
        <!--Caja para agregar secciones-->
            <section >
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2f/Google_2015_logo.svg/1200px-Google_2015_logo.svg.png" alt="Logo de Google" class="main-logo">
            </section>
        <!--SECTION INPUT-->
        <section class="main-input">
            <!-- DIVISIÓN-Cajita redondeada-->
            <div class="main-input-container">
                <span class="search-icon"> </span>
                <!--INPUT RADIO Y CHECKBOX-->
                <!--<input type="radio">-->
                <input type="text">
                <a class="micro-icon" href=""></a>
                <a class="cam-icon" href=""></a>
            </div>
            
        </section>

    </main>
</body>
</html>

body {
    /* Margen predeterminado en las páginas web */
    margin: 0;
    /* Margen pa dentro */
    padding: 0;
    /* Tamaño de fuente */
    font-size: 12px;
    /* Fuente de texto */
    font-family: Arial, Helvetica, sans-serif;
}

/* NAVEGACIÓN */
header {
    width: 100%;
    height: 50px;
}

header nav{
    display:flex;
    /*Mover mi nav hacia la derecha*/
    justify-content: flex-end;
    margin-right: 10px;
}

header nav .nav-right-section
{
/* Eliminar viñetas*/
list-style: none;
width: 250px;
/*Hacemos el elemento flexible*/
display: flex;
/*Centramos*/
justify-content: space-between;
/*Centrado vertical*/
align-items: center;
height: auto;
}

nav .nav-right-section a {
    text-decoration: none;
    color:rgb(0, 0, 0, .87)
}

nav .nav-right-section .menu { 

    background-image: url('/Images/puntitos.png');
    width: 20px;
    height: 20px;
    /* Tamaño de la imagen de fondo contenido */
    background-size: contain;
    background-repeat: no-repeat;
    /* Posicionar la imagen al centro */
    background-position: center;
}

.fotoE {
    border-radius: 100%;
}

main {
    margin-top: 100px;
    /*CENTRAR ELEMENTOS*/
    text-align: center;
}

main .main-logo {
    width: 300px;
    margin: 0 auto;
}

/*INPUT SECTION*/
main .main-input {

    width: 500px;
    margin: 0 auto;
}

main .main-input-container {
    margin-top: 33px;
    width: 500px;
    border: 1px solid #cbcbcb;
    border-radius: 50px;
}

main .main-input-container input {
    height: 35px;
    border: none;
    outline: none;
    width: 390px;
}

main .main-input-container .search-icon {
    background-image: url("https://seekicon.com/free-icon-download/search_20.svg");
    background-size: contain;
    background-position: center;
    padding-left: 50px;
    background-repeat: no-repeat;
    width: 25px;
    height: 25px;
}

main .main-input .micro-icon {
    background-image: url("http://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Google_mic.svg/726px-Google_mic..png");
    background-size: contain;
    background-position: center;
    padding-right: 10px;
    background-repeat: no-repeat;
    
}

main .main-input .cam-icon {
    background-image: url("https://static.vecteezy.com/system/resources/previews/028/766/357/original/google-camera-lens-icon-symbol-free-png.png");
    background-size: contain;
    background-position: center;
    padding-right: 40px;
    background-repeat: no-repeat;
    
}
