<script>
  export default {
    data: () => ({
      contador: 500,
    }),
    methods: {
      saludar(){
        console.log("hola 10a ! @");
      },
      incrementar(){
        this.contador++;
      },
      disminuir(){
        this.contador--;
      },
      reset(){
        this.contador = 500;
      },
    }
  };

</script>
<template>
  <!-- German Martinez Correo -->
  <img src="./assets/logo.svg" alt="Logo VUE" width="125" height="125">
<div class="container">
  <small>
    <h1>Hola desde VUE.JS 3</h1>
  </small>
  <hr>
  <h2>Contador {{ contador }}</h2>
  <button @click="incrementar()">+1</button>
  <button @click="disminuir()">-1</button>
  <button @click="reset()">RESET</button>
</div>
</template>

<style scoped>
  .container{
    text-align: center;

  }
  small{
    color: #666;
  }
  h1{
    font-weight: bolder;
  }
  h2{

    font-size: 2.5rem;
  }
  button{
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0px 8px;
  }
</style>