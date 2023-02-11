<script>
</script>

<svelte:head>
  <script
    src="https://kit.fontawesome.com/2da7ac124d.js"
    crossorigin="anonymous"
  ></script>
</svelte:head>

<main>
  <section id="sp-top-bar">
    <div class="container">
      <div class="row">
        <div id="sp-top1" class="col-xs-12 col-sm-6 col-md-6">
          <div class="sp-column ">
            <ul class="social-icons">
              <li><i class="fa fa-facebook"/></li>
              <li><i class="fa fa-twitter"/></li>
              <li><i class="fa fa-youtube"/></li>
              <li><i class="fa fa-flickr"/></li>
              <li><i class="fa fa-flickr"/></li>
              <li><i class="fa fa-instagram"/></li>
            </ul>
          </div>
        </div>
        <div id="sp-top2" class="col-xs-12 col-sm-6 col-md-6">
          <div class="sp-column ">
            <ul class="sp-contact-info">
              <li class="sp-contact-phone">
                <i class="fa fa-phone" aria-hidden="true" />
                <a href="tel:925284043">925284043</a>
              </li>
              <li class="sp-contact-email">
                <i class="fa fa-envelope" aria-hidden="true" />
                <a href="mailto:45003875.ies@edu.jccm.es"
                  >45003875.ies@edu.jccm.es</a
                >
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>
</main>

<style>
  #sp-top-bar {
    background-color: #f5f5f5;
    color: #999999;
  }
  #sp-top-bar {
    padding: 8px 0;
  }
  .container {
    padding-right: 0.938;
    padding-left: 0.938;
    margin-right: auto;
    margin-left: auto;
  }
  ul {
    display: block;
    list-style-type: disc;
  }
  ul.social-icons > li {
    display: inline-block;
    margin: 5px 7px;
  }
  ul.social-icons > li a {
    color: #999999;
  }
  ul.social-icons {
    list-style: none;
    padding: 0;
    display: inline-block;
  }
  main,
  section {
    display: block;
  }
  li {
    list-style: none;
  }
  .sp-contact-info li {
    display: inline-block;
    margin: 0 10px;
    font-size: 90%;
  }
  a {
    color: #22b8f0;
  }
  a,
  a:hover,
  a:focus,
  a:active {
    text-decoration: none;
  }
</style>
