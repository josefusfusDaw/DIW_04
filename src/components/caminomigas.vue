<template>
  <section id="camino-migas">
      <a class="inicio" href="#"> Inicio </a> >
      <a href="#">Iphone </a> > 
      <a class="actual" href="#">Iphone 13 Pro</a> 


  </section>
</template>

<script>
export default {
    name:'migas',
  props: {
    msg: String
  }
}
</script>

<style>
section#camino-migas {
    margin-left: 1rem;
    display:flex;

}
section#camino-migas a, 
section#camino-migas a:hover, 
section#camino-migas a:visited{
    text-decoration: none;
    font-size: 1.2rem;
    margin-left: 1rem;
    margin-right: 1rem;
    color: #020202;
}
section#camino-migas a.actual {
    font-weight: 700;
}
section#camino-migas {
    margin-left: 1rem;
    color: #020202;
}
</style>