<script>
  import Nav from "../components/Nav.svelte";
  import Hero from "../components/Hero.svelte";
  import Footer from "../components/Footer.svelte";

  export let segment;
</script>

<style>
  .wrap {
    max-width: 1024px;
    margin: auto;
    font-family: "Microsoft JhengHei";
    color: #3d1101;
  }
  .header {
    background-color: #000;
    color: #fff;
    width: 100%;
    position: relative;
  }
  .Banner {
    width: 100%;
    height: 420px;
    background-image: url(/header_desktop.png);
    background-position: center center;
    background-repeat: no-repeat;
  }
  .container {
    width: 100%;
    background-color: #efe9e7;
  }
  @media (max-width: 600px) {
    .Banner {
      background-image: url(/header_mobile.png);
    }
  }
</style>

<div class="wrap">
  <div class="header">
    <div class="Banner">
      <Nav {segment} />
      <Hero />
    </div>
  </div>
  <div class="container">
    <slot />
  </div>
  <Footer />
</div>
