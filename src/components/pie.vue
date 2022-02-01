<template>
    <footer id="pie">
    <p>© Copyright 2022 - Todos los derechos reservados </p>


  </footer>
</template>

<script>
export default {
name: 'pie',
  props: {
    msg: String
  }
}
</script>

<style>
#pie {
    background-color: #333333;
}
#pie p {
    padding: 2rem 1rem;
    color: white;
    text-align: center;
    
}
</style>