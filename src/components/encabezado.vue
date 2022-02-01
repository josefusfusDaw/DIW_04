<template>
          <header>
                <!-- ENCABEZADO -->
                <div class="flex-header">

                    <div class="logo">
                       <img src="../assets/logo_apple.png" class="logo_cabecera" alt="Logo Apple" copyright="c Apple, Inc" />
                       <img src="../assets/logo_apple.png" class="logo_cabecera" alt="Logo Apple" copyright="c Apple, Inc" />
                    <h1>APPLES</h1>
                    </div>
                    <div class="nav">
                        <nav>
                            <ul class="nav_links">
                                <li><a href="#">Inicio</a></li>
                                <li><a href="#">Mac</a></li>
                                <li><a href="#">Iphone</a></li>
                                <li><a href="#">Ipad</a></li>
                                <li><a href="#">Accesorios</a></li>
                            </ul>

                        </nav>
                    </div>
                    <div class="botonAcceso">
                        <a class="botonLogin" href="#">Registro</a>
                        <a class="botonLogin" href="#">Identificate</a>
                    </div>
                </div>

            </header>
</template>

<script>
export default {
  name: "encabezado",
  props: {
    msg: String,
  },
};
</script>

<style>

.logo_cabecera {
  width: 150px;
  height: 150px;
  
}



.logo{
    display: flex;
    flex-direction: row;
    align-items: flex-end;
    background-color: #fffbfb;
   
}

.flex-header{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    font-size: 25px;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: bold;
    align-items: flex-end;

    
}

.head-derecha{
    display: flex;
    flex-direction: row;
   
}

.flex-header nav{
  
    text-decoration: none;
    font-size: 25px;

    
}

.nav{
    display: flex;
    background-color: #fffbfb;
    align-items: flex-end;
    justify-content: space-between;
    margin-left: auto;
    margin-right: auto;
}
.nav_links{
    list-style: none;
    padding-left: 1em;
    padding-right: 1em;
}

li, a {
    color: #020202;
    text-decoration: none;
}
.nav_links li{
    display: inline-block;
     padding: 5px;
}

.nav_links li a{
    transition: all 0.3s ease 0s;
}

.nav_links li a:hover{
    color:rgb(144, 144, 146) 
}

/*
.nav_links li a:visited{
    color:#C9C217;
}*/

.botonAcceso{
    background-color: #fffbfb;
    display: flex;
    flex-direction: row;
    align-items: flex-end;
    padding: 20px;
    color: rgb(144, 144, 146) ;
    justify-content: flex-end;
    height: fit-content;
}

.botonLogin{

    background-color: #000000;
    border-radius: 20px;
    font-size:xx-large ;
    color: #fffbfb;
    cursor: pointer; 
    vertical-align: center;
    justify-content: center;
    border-width: 0px;
    display: inline-block;
    padding: 2px;
    
}
</style>