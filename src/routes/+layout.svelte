<script>
  import Contacto from "../lib/contacto.svelte";
  import Footer from "../lib/footer.svelte";
  import Header from "../lib/header.svelte";
</script>

<main>
    <Contacto/>
    <Header/>
    <slot/>
    <Footer/>
</main>

<style lang="sass">
  
</style>
