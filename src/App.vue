<script>
  export default {
    data: () => ({
      contador : 500,
    }),
    methods: {
      saludar(){
        console.log("Hola 10A");
      },
      incrementar(){
        this.contador++;
      },
      restar(){
        this.contador--;
      },
      resetear(){
        this.contador = 10;
      }
    }
  };
</script>
<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Luis Enrique Montiel Rojas 10°A DGS</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Pagina 1</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Pagina 2</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  <img class="imglog" src="./assets/logo.svg" alt="Logo VUE" width="125" />
  <div class="container">
    <small>
      <h1>Hola desde VUE.js</h1>
    </small>
    <hr />
    <h2>Contador {{contador}}</h2>
    <button v-on:click="incrementar()">+1</button>
    <button v-on:click="restar">-1</button>
    <button v-on:click="resetear()">Reset</button>
  </div>
</template>

<style scoped>
  .container{
    text-align: center;
    margin-top: 60px;
  }
  .imglog{
    margin-top: 60px;
  }
  small{
    color: #666;
  }
  h1 {
    color: bolder;
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
