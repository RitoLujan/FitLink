<template>
  <header>
    <FitLinkNavbar />
  </header>
  <body>
    <div class="container">
      <h1>BIENVENIDO A FITLINK</h1>
    </div>
    <div id="carouselExampleDark" class="carousel slide">
      <div class="carousel-indicators">
        <button
          type="button"
          data-bs-target="#carouselExampleDark"
          data-bs-slide-to="0"
          class="active"
          aria-current="true"
          aria-label="Slide 1"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleDark"
          data-bs-slide-to="1"
          aria-label="Slide 2"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleDark"
          data-bs-slide-to="2"
          aria-label="Slide 3"
        ></button>
      </div>
      <div class="carousel-inner">
        <div class="carousel-item active" data-bs-interval="10000">
          <img src="../assets/forma.jpg" class="d-block w-100" />
          <div class="carousel-caption d-none d-md-block">
            <h5>Ejercicios Recomendados</h5>
            <p>De la mano de los mejores, para que logres tus objetivos.</p>
          </div>
        </div>
        <div class="carousel-item" data-bs-interval="2000">
          <img src="../assets/musculo.jpg" class="d-block w-100" />
          <div class="carousel-caption d-none d-md-block">
            <h5>Planes de entrenamiento</h5>
            <p>
              Contamos con los mejores planes de ejercicios, para que alcances
              tus objetivos.
            </p>
          </div>
        </div>
        <div class="carousel-item">
          <img src="../assets/peso.jpg" class="d-block w-100" />
          <div class="carousel-caption d-none d-md-block">
            <h5>Planes Alimenticios</h5>
            <p>Las mejores dietas a tu alcance, para lograr tus metas</p>
          </div>
        </div>
      </div>
      <button
        class="carousel-control-prev"
        type="button"
        data-bs-target="#carouselExampleDark"
        data-bs-slide="prev"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Anterior</span>
      </button>
      <button
        class="carousel-control-next"
        type="button"
        data-bs-target="#carouselExampleDark"
        data-bs-slide="next"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Siguiente</span>
      </button>
    </div>
    <div class="container">
      <h2 style="margin-bottom: 20px">Formulario de Suscripción</h2>
      <form action="#" method="post">
        <div class="form-group">
          <input
            type="email"
            id="email"
            name="email"
            placeholder="email@example.com"
            required
          />
          <button type="submit">Suscribirse</button>
        </div>
      </form>
      <p id="message">¡Gracias por suscribirte!</p>
    </div>
    <h1>Nuestros servicios</h1>
    <div class="row row-cols-1 row-cols-md-3 g-4" style="margin: 20px;">
      <div class="col">
        <div class="card h-100">
          <img src="../assets/ejercicio.jpg" class="card-img-top" alt="..." />
          <div class="card-body">
            <h5 class="card-title">Ejercicios que se adecuan a todo tipo de objetivos</h5>
            <p class="card-text">
              Con nuestros expertos encontraras todo tipo de ejercicios que se
              adecuan a tus necesidades y al equipo que tienes a ti alcance. <br>
              ¡Sin la necesidad de atarte a un plan riguroso!
            </p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card h-100">
          <img src="../assets/rutina.jpg" class="card-img-top" alt="..." />
          <div class="card-body">
            <h5 class="card-title">Plan de ejercicios adecuados para tus objetivos</h5>
            <p class="card-text">
              De la mano de nuestros expertos encontraras y llevaras un control mas efectivo
              sobre tus rutinas de entrenamiento.<br>
              ¡En poco tiempo veras resultados!
            </p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card h-100">
          <img src="../assets/alimentacion.jpg" class="card-img-top" alt="..." />
          <div class="card-body">
            <h5 class="card-title">Planes Alimenticios</h5>
            <p class="card-text">
              Somos concientes que la parte mas complicada para lograr tus metas es lidiar con los antojitos,
              por eso implementamos nuestras nuevas dietas bastante variadas.
            </p>
          </div>
        </div>
      </div>
    </div>
  </body>
  <footer>
    <FitLinkFooter />
  </footer>
</template>

<script>
import FitLinkNavbar from "./FitLinkNavbar.vue";
import FitLinkFooter from "./FitLinkFooter.vue";

export default {
  name: "FitLinkMenu",
  components: {
    FitLinkNavbar,
    FitLinkFooter,
  },
};
</script>

<style>
body {
  font-family: sans-serif;
  margin: 0;
  padding: 0;
}

.carousel {
  margin: 20px auto;
}

.container {
  width: 500px;
  margin: 0 auto;
  text-align: center;
}

h1 {
  margin-top: 20px;
  margin-bottom: 20px;
}

h2 {
  margin-top: 20px;
  margin-bottom: 20px;
  text-align: center;
  font-size: 24px;
  color: #333;
}

.form-group {
  display: flex;
  margin-bottom: 20px;
}

label {
  margin-right: 10px;
}

input[type="email"] {
  flex: 1;
  padding: 10px;
  border: 1px solid #ccc;
}

button {
  background-color: #007bff;
  color: white;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
}

#message {
  color: green;
}

img {
  width: 80%;
  height: auto;
}
</style>
