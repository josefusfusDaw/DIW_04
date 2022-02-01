<template>
  <section id="producto-descripcion">
    <h1>DESCRIPCIÓN DEL PRODUCTO</h1>
    <ul>
      <li>Nuevo Iphopne 13 Pro</li>
      <li>
        El Apple iPhone 13 Pro representa una actualización del iPhone 12.
        Conservando la pantalla OLED de 6.1 pulgadas, el iPhone 13 cuenta con un
        procesador Apple A15 Bionic, con opciones de almacenamiento de 128GB.
        256GB. o 512GB. La cámara principal del iPhone 13 es dual, con lentes
        wide y ultrawide de 12MP con IBIS y zoom óptico 2x, y la cámara frontal
        es de 12MP. El iPhone 13 tiene parlantes stereo, soporta carga rápida
        tanto por cable como inalámbrica, es resistente al polvo y agua, y
        soporta redes 5G.
      </li>
    </ul>
  </section>
  <section>
    <video width="640" height="480" controls>
      <source
        src="../assets/images/videoiphone.mp4"
        type="video/mp4"
        alt="Video publicitario iphone 13"
      />
     Tu navegador no soporta video
    </video>
  </section>
</template>

<script>
export default {
  name: "cuerpo",
  props: {
    msg: String,
  },
};
</script>

<style>
#producto-descripcion {
  margin: 1rem;
}
#producto-descripcion h1 {
  color: #020202;
}
</style>