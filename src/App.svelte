<script lang="ts">
  import foto from './assets/logo_principal_jpg.jpg'
  import Footer from './Footer.svelte';
  import SobreMi from './SobreMi.svelte';
  import MiStack from './miStack.svelte';
  import MiTrivia from './miTrivia.svelte';
</script>

<style>
  .navegator{
    background: rgb(23,22,30);
    background: linear-gradient(45deg, rgba(23,22,30,1) 0%, rgba(65,64,94,1) 100%);
  }
</style>

<header class="navegator sticky-top">
  <div class="container">
    <div class="d-flex flex-wrap justify-content-center">
      <a href="/" class="d-flex align-items-center mb-2 mb-lg-0 text-white text-decoration-none">
        <img height="60" width="134.44" src="{foto}" alt="">
      </a>

      <ul class="nav col-12 col-lg-auto me-lg-auto mb-2 justify-content-center mb-md-0">
        <li><a href="#" class="nav-link px-2 text-white">Sobre Mí</a></li>
        <li><a href="#" class="nav-link px-2 text-white">Mi Portafolio</a></li>
      </ul>

    </div>
  </div>
</header>

<SobreMi></SobreMi>

<MiStack></MiStack>

<MiTrivia></MiTrivia>

<Footer></Footer>