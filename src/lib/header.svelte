<script>
</script>

<svelte:head>
  <script
    src="https://kit.fontawesome.com/2da7ac124d.js"
    crossorigin="anonymous"
  ></script>
</svelte:head>

<main>
  <div class="container">
    <div class="row">
      <div class="col-3 logo"><img src="img/logo.png" alt="logo IES Azarquiel" /></div>
      <div class="col-9">
        <ul>
          <li class="inicio responsivo">INICIO</li>
          <li class="responsivo">AL DÍA <i class="fa-solid fa-angle-down" /></li>
          <li class="responsivo">EL LORO</li>
          <li class="responsivo">EL CENTRO <i class="fa-solid fa-angle-down" /></li>
          <li class="responsivo">SECRETARÍA <i class="fa-solid fa-angle-down" /></li>
          <li class="responsivo">FAMILIAS <i class="fa-solid fa-angle-down" /></li>
          <li class="responsivo">BOLSA</li>
          <li>
            <div class="offcanvas offcanvas-end" id="demo">
              <div class="offcanvas-header">
                <h3 class="offcanvas-title">SEARCH</h3>
                <button type="button" class="btn-close boton-cerrar" data-bs-dismiss="offcanvas"></button>
              </div>
              <div class="form-group">
                <input type="text" class="form-control centrar-input" aria-describedby="emailHelp" placeholder="Search ...">
              </div>
              <div class="offcanvas-body">
                <ul class="lista-desplegable">
                  <li><i class="fa-solid fa-chevron-right"></i> INICIO</li>
                  <li><i class="fa-solid fa-chevron-right"></i> AL DÍA</li>
                  <li><i class="fa-solid fa-chevron-right"></i> EL LORO</li>
                  <li><i class="fa-solid fa-chevron-right"></i> EL CENTRO</li>
                  <li><i class="fa-solid fa-chevron-right"></i> SECRETARÍA</li>
                  <li><i class="fa-solid fa-chevron-right"></i> FAMILIAS</li>
                  <li><i class="fa-solid fa-chevron-right"></i> BOLSA</li>
                </ul>
              </div>
            </div>

            <div class="container-fluid mt-3">
              <button
                class="btn centrar"
                type="button"
                data-bs-toggle="offcanvas"
                data-bs-target="#demo"
              >
                <i class="fa-solid fa-bars" />
              </button>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</main>

<style lang="sass">
  .container
    margin-top: 1rem
    margin-bottom: 1rem
    top: 0px
    position: sticky
  ul
    display: flex
    align-items: center
    justify-content: center
  li
    list-style: none
    margin: 0 1.5rem 0 0
    color: #000
    transition: 0.2s ease-in-out
    cursor: pointer
    &:hover
      color: #22b8f0
  .inicio
    color: #22b8f0
  a
    color: #000
    transition: 0.2s ease-in-out
    text-decoration: none
    &:hover
      color: #22b8f0
  .logo
    width: 25%
  img
    max-width: 100%
  .centrar
    margin-top: -1rem
  h3
    font-size: 1rem
  .offcanvas
    background-color: rgba(0,0,0,0.7)
    color: white
  .boton-cerrar
    color: white
    background-color: white
    transition: 0.2s ease-in-out
  .centrar-input
    width: 80%
    margin-top: 2rem
    margin-left: 10%
    background: transparent
    border-color: #5f5f5f
    color: white
    &::placeholder
      color: #5f5f5f
  .lista-desplegable
    display: flex
    flex-direction: column
    justify-content: center
    align-items: flex-start
  .lista-desplegable li
    list-style: none
    margin-top: 0.5rem
    margin-bottom: 0.5rem
    color: white
  @media (max-width: 1200px) 
    .responsivo
      display: none
</style>
