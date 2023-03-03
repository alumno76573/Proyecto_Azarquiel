<script>
  import FlipCard from "../lib/flipCard.svelte";


</script>

<main>
    <div class="container d-flex">
        <div class="row">
            <div class="col-xl-6">
                <FlipCard 
                    src="./img/pexels-lucie-liz-3165335.jpg" 
                    alt="imagen desarrollo de videojuegos" 
                    title="Desarrollo de videojuegos y Realidad virtual"
                    url="/videojuegos"/>
            </div>
            <div class="col-xl-6">
                <FlipCard
                    src="./img/pexels-tima-miroshnichenko-5380792.jpg"
                    alt="imagen ciberseguridad"
                    title="Ciberseguridad"
                    url="/ciberseguridad"/>
            </div>
        </div>
    </div>
</main>

<style lang="sass">
    main
        margin-bottom: 2rem
    .container
        display: flex
        justify-content: space-around
        padding: 0
    .row
        padding: 0
        margin: 0
</style>
