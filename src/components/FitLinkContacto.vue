<template>
    <header>
        <FitLinkNavbar/>
    </header>
    <body>
        <div class="container">
        <h1>CONTÁCTANOS</h1>
        <form>
            <div class="mb-3">
                <label for="name" class="form-label">Nombre</label>
                <input type="text" class="form-control" id="name" placeholder="Ingresa tu nombre">
            </div>
            <div class="mb-3">
                <label for="email" class="form-label">Email</label>
                <input type="email" class="form-control" id="email" placeholder="Ingresa tu email">
            </div>
            <div class="mb-3">
                <label for="subject" class="form-label">Asunto</label>
                <input type="text" class="form-control" id="subject" placeholder="Escribe el asunto">
            </div>
            <div class="mb-3">
                <label for="message" class="form-label">Mensaje</label>
                <textarea class="form-control" id="message" rows="3" placeholder="Escribe tu mensaje aqui"></textarea>
            </div>
            <button type="submit" class="btn btn-primary">Enviar</button>
        </form>
    </div>
    </body>
    <footer>
        <FitLinkFooter/>
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

</style>