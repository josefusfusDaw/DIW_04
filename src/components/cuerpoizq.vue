<template>
<link href="https://fonts.googleapis.com/icon?family=Material+Icons"
      rel="stylesheet">
<section class="productocompra">
  <article id="producto-imagen">
    <div class="img-big">
      <img v-bind:src="fotos[0]" alt="Iphone 13" />
    </div>
    <div class="img-mini">
      <a @click="cambiarFoto(1)"
        ><img v-bind:src="fotos[1]" alt="Iphone 13" copyright="c Apple, Inc"
      /></a>
      <a @click="cambiarFoto(2)"
        ><img v-bind:src="fotos[2]" alt="Iphone 13" copyright="c Apple, Inc"
      /></a>
      <a @click="cambiarFoto(3)"
        ><img v-bind:src="fotos[3]" alt="Iphone 13" copyright="c Apple, Inc"
      /></a>
      <a @click="cambiarFoto(4)"
        ><img v-bind:src="fotos[4]" alt="Iphone 13" copyright="c Apple, Inc"
      /></a>
    </div>
  </article>
   <article id="producto-datos">
      <h1>Iphone 13 Pro</h1>
      <h2>1350,00 € <span class="iva">sin IVA: 1066,50€</span></h2>
      <div class="wrapper">
          <button class="btn" @click="cambiarContador('-1')" type="button" name="button">-</button>
          <input class="cantidad" type="text" name="name" :value="contador">
          <button class="btn" @click="cambiarContador('1')" type="button" name="button">+</button>
      </div>
      <br>
      <button class="boton"><span class="material-icons">add_shopping_cart</span> AÑADIR</button>
   </article>
   </section>
</template>  

<script>
export default {
  name: "cuerpoizq",
    data () {
        return {
            fotos: [
                require ('../assets/images/iphone13_1.jpeg'),
                require ('../assets/images/iphone13_1.jpeg'),
                require ('../assets/images/iphone13_2.jpeg'),
                require ('../assets/images/iphone13_3.jpeg'),
                require ('../assets/images/iphone13_4.jpeg')],
            contador: 1
        }
    },
    methods: {
        cambiarFoto(id) {
            this.fotos[0] = this.fotos[id]
        },
         cambiarContador(num) {
            this.contador += +num;
            if (!isNaN(this.contador) && (this.contador < 0)) {
              this.contador = 0
            }
        }
    }
}    
</script>

<style escoped>
#producto-imagen {
    border-radius: 25px;
    padding: 1rem;
    margin: 1rem;
    flex: 1 0 50%;
    
    
}


.img-mini {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
}
.img-mini img {
    width: 100px;
    border:2px solid #d8d8d8;
    
}

.productocompra{
    display: flex;
    flex-direction: row;
}

section#producto-datos {
  flex: 1 1 18rem;
}
h1 {
  font-size: 2.2rem;
}
h2 {
  font-size:1.7rem;
  color: #020202;
}
span.iva {
  font-size:1rem;
  font-weight: normal;
  color: #282828
}
.wrapper {
  height: 2rem;
  display: flex;
}

.cantidad {
  border: none;
  text-align: center;
  width: 2rem;
  font-size: 1.2rem;
  border: 1px solid #d8d8d8;
}
.btn {
  border: 1px solid #d8d8d8;
  width: 1.8rem;
}
button:focus, input:focus {
  outline: 0;
}

</style>