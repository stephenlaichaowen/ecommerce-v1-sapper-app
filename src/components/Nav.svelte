<script>
  export let segment;
  let menuShow = false

  function toggleMenu() {
    menuShow = !menuShow
    console.log(`menu status: ${menuShow}`)
  }
</script>

<style>
  .top {
    height: 56px;
    width: 100%;
    background-color: rgba(0, 0, 0, 0.5);
    opacity: 20;
    /* display: flex;
    justify-content: space-between; */
  }
  .nav {
    float: right;
    /* padding-top: 18px; */
  }
  @media (max-width: 575px) {
    .nav {
      background: transparent;
      max-width: 575px;
      max-height: 0px;
      overflow: hidden;
      transition: max-height 0.5s;
      height: auto;
      z-index: 110;
      position: absolute;
      right: 0;
      top: 30px;
    }
  }
  .nav li {
    display: inline-block;
    font-size: 18px;
    margin-right: 50px;
  }
  @media (max-width: 575px) {
    .nav li {
      margin-right: 10px;
    }
  }
  .nav li a {
    text-decoration: none;
    color: #fff;
  }
  .nav li a:hover {
    color: #ff5809;
  }
  .showmenu {
    display: none;
    font-size: 30px;
  }
  @media (max-width: 575px) {
    .showmenu {
      display: block;
      position: absolute;
      top: 5px;
      right: 12px;
      color: #fff;
    }
  }
  .logo {
    float: left;
    margin-left: 20px;
    padding-top: 8px;
  }

  @media (max-width: 575px) {
    .menuShow {
      max-height: 500px;
    }
  }
</style>

<div class="top">
  <div class="logo">
    <h1>
      <a href="/" aria-current={segment === undefined ? 'page' : undefined}>
        <img class="logo" src="/logo_w(null).svg" alt="" />      
      </a>    
    </h1> 
    <!-- <h1><img class="logo" src="/logo_w(null).svg" alt="" /></h1>  -->
  </div>
  <ul class="nav">
    <li>
      <a aria-current={segment === 'order' ? 'page' : undefined} href="/order">
        線上訂購
      </a>
    </li>
    <li>
      <a aria-current={segment === 'login' ? 'page' : undefined} href="/login">
        登入
      </a>
    </li>
    <li>
      <a
        aria-current={segment === 'register' ? 'page' : undefined}
        href="/register">
        註冊
      </a>
    </li>
  </ul>
  <span on:click|preventDefault={toggleMenu} class="showmenu" class:menuShow={menuShow}>
    <i class="fa fa-bars" aria-hidden="true" />
  </span>
</div>
