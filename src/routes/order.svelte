<script>
  let item1 = true
  let item2 = true
  let item3 = true
  let item4 = true
  let item5 = true
  let item6 = true
  let item7 = true

  function toggleItem1() { item1 = !item1 }
  function toggleItem2() { item2 = !item2 }
  function toggleItem3() { item3 = !item3 }
  function toggleItem4() { item4 = !item4 }
  function toggleItem5() { item5 = !item5 }
  function toggleItem6() { item6 = !item6 }
  function toggleItem7() { item7 = !item7 }
  
</script>

<style>
  .order {
    padding-top: 5%;
    padding-bottom: 5%;
    overflow: auto;
    background-color: #efe9e7;
    font-size: 16px;
  }
  .menu {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  }
  .order a {
    color: #3d1101;
  }
  .order .slider {
    width: 17%;
    float: left;
    padding-left: 5%;
    margin-right: 3%;
  }
  ul {
    margin: 0;
    padding: 0;
  }
  li {
    /* padding: 0; */
    list-style-type: none;
  }
  @media (max-width: 414px) {
    .order .slider {
      width: 95%;
      margin-right: 0;
      padding-left: 2.5%;
      padding-right: 2.5%;
      padding-top: 30px;
    }
  }
  .order .slider i {
    font-size: 32px;
    margin-right: 5px;
  }
  .order .slider ul {
    margin-top: 30px;
  }
  .order .slider ul li {
    line-height: 35px;
    border-bottom: 1px solid #3d1101;
    cursor: pointer;
    padding-left: 10px;
  }
  .order .slider .current {
    background-color: #3d1101;
    color: #fff;
  }
  .order .chart {
    width: 71%;
    padding-right: 4%;
    float: right;
    overflow-y: hidden;
  }
  @media (max-width: 414px) {
    .order .chart {
      width: 95%;
      padding-left: 2.5%;
      padding-right: 2.5%;
    }
  }
  .order .chart .search {
    width: 60%;
    margin-bottom: 20px;
    display: inline-block;
  }
  @media (max-width: 414px) {
    .order .chart .search {
      width: 100%;
      margin-top: 30px;
    }
  }
  .order .chart .search > div {
    width: 100%;
    border: 1px solid #3d1101;
    height: 24px;
  }
  .order .chart .search input[type="text"] {
    background-color: transparent;
    height: 22px;
    float: left;
    border: 0px;
    width: 85%;
  }
  .order .chart .search i {
    font-size: 20px;
    height: 22px;
    width: 15%;
    background: #3d1101;
    color: #fff;
    text-align: center;
    padding-top: 2px;
  }
  .order .chart .search i:hover {
    background: #f75000;
  }
  .order .chart .pay {
    width: 35%;
    display: inline-block;
    text-align: right;
    vertical-align: top;
  }
  @media (max-width: 414px) {
    .order .chart .pay {
      width: 100%;
      margin-bottom: 40px;
    }
  }
  .order .chart .pay span {
    margin-left: 8px;
    margin-right: 10px;
  }
  .order .chart .pay i {
    font-size: 30px;
  }
  .order .chart .pay i:hover {
    color: #f75000;
  }
  .order .chart .menu {
    width: 100%;
    height: auto;
  }
  .order .chart .menu .menu-1 {
    display: block;
  }
  .order .chart .menu .menu-2 {
    display: block;
  }
  .order .chart .menu .menu-3 {
    display: block;
  }
  .order .chart .menu .product {
    width: 210px;
    box-shadow: 4px 4px 3px rgba(51, 51, 102, 0.5);
    margin-bottom: 30px;
    border: 1px solid #d0d0d0;
    padding-bottom: 20px;
    margin-right: 3%;
    position: relative;
  }
  @media (max-width: 414px) {
    .order .chart .menu .product {
      width: 100%;
    }
  }
  .order .chart .menu .product .far {
    position: absolute;
    top: 8px;
    left: 8px;
    color: #fff;
    font-size: 25px;
    cursor: pointer;
  }
  .order .chart .menu .product .fas {
    position: absolute;
    top: 8px;
    left: 8px;
    color: #fff;
    font-size: 25px;
    cursor: pointer;
    /* visibility: hidden; */
  }
  .order .chart .menu .product img {
    width: 100%;
    height: 120px;
    margin-bottom: 15px;
  }
  .order .chart .menu .product ul li {
    text-align: center;
    width: 100%;
    position: relative;
  }
  .order .chart .menu .product .product-C {
    font-size: 20px;
    margin-bottom: 5px;
  }
  .order .chart .menu .product .product-E {
    font-size: 12px;
    margin-bottom: 40px;
  }
  .order .chart .menu .product .product-E::after {
    position: absolute;
    content: " ";
    height: 5px;
    width: 50%;
    bottom: -120%;
    left: 25%;
    border-bottom: 1px solid #3d1101;
  }
  .order .chart .menu .product .price {
    font-size: 20px;
    margin-bottom: 20px;
  }
  .order .chart .menu .product .price span {
    font-weight: bold;
  }
  .order .chart .menu .product input[type="submit"] {
    width: 80%;
    background-color: transparent;
    border: 2px solid #f75000;
    border-radius: 3px;
    color: #f75000;
    font-size: 16px;
    padding-left: 10%;
    cursor: pointer;
  }
  .order .chart .menu .product input[type="submit"]:hover {
    background-color: #f75000;
    color: #fff;
  }
  .order .chart .menu .product i {
    position: absolute;
    font-size: 18px;
    top: 15%;
    left: 25%;
    color: #f75000;
  }
</style>

<svelte:head>
  <title>Order</title>
</svelte:head>

<div class="order">
  <div class="slider">
    <i class="fa fa-leaf" aria-hidden="true" />
    <span>線上訂購美食</span>
    <ul>
      <li class="select-Mall current">全部(23)</li>
      <li class="select-M1">只愛吃薯條(18)</li>
      <li class="select-M2">加熱就可食(1)</li>
      <li class="select-M3">不敗漢堡系列(4)</li>
    </ul>
  </div>
  <div class="chart">
    <div class="search">
      <div>
        <input type="text" />
        <a href="#/">
          <i class="fa fa-search" aria-hidden="true" />
        </a>
      </div>
    </div>
    <div class="pay">
      結帳去
      <span>|</span>
      <a href="#/">
        <i class="fa fa-shopping-cart" aria-hidden="true" />
      </a>
    </div>
    <div class="menu">
      <div class="product menu-1">
      {#if item1}
        <i class="far fa-heart fa-3x" aria-hidden="true" on:click={toggleItem1} />
      {:else}
        <i class="fas fa-heart fa-3x" aria-hidden="true" on:click={toggleItem1} />
      {/if}
        <img src="/product11.jpg" alt="" />
        <ul>
          <li class="product-C">經典薯條</li>
          <li class="product-E">Classic Hamburger Package</li>
          <li class="price">
            $
            <span>999</span>
          </li>
          <li class="shopcart">
            <input type="submit" value="加入購物車" />
            <i class="fa fa-shopping-cart" aria-hidden="true" />
          </li>
        </ul>
      </div>
      <div class="product menu-1">
        {#if item2}
          <i class="far fa-heart" aria-hidden="true" on:click={toggleItem2} />
        {:else}
          <i class="fas fa-heart" aria-hidden="true" on:click={toggleItem2} />
        {/if}
        <img src="/product12.jpg" alt="" />
        <ul>
          <li class="product-C">波浪薯條</li>
          <li class="product-E">Classic Hamburger Package</li>
          <li class="price">
            $
            <span>1,999</span>
          </li>
          <li class="shopcart">
            <input type="submit" value="加入購物車" />
            <i class="fa fa-shopping-cart" aria-hidden="true" />
          </li>
        </ul>
      </div>
      <div class="product menu-2">
        {#if item3}
          <i class="far fa-heart" aria-hidden="true" on:click={toggleItem3} />
        {:else}
          <i class="fas fa-heart" aria-hidden="true" on:click={toggleItem3} />
        {/if}
        <img src="/product10.jpg" alt="" />
        <ul>
          <li class="product-C">加熱就可食套餐</li>
          <li class="product-E">Classic Hamburger Package</li>
          <li class="price">
            $
            <span>10</span>
          </li>
          <li class="shopcart">
            <input type="submit" value="加入購物車" />
            <i class="fa fa-shopping-cart" aria-hidden="true" />
          </li>
        </ul>
      </div>
      <div class="product menu-3">
        {#if item4}
          <i class="far fa-heart" aria-hidden="true" on:click={toggleItem4} />
        {:else}
          <i class="fas fa-heart" aria-hidden="true" on:click={toggleItem4} />
        {/if}
        <img src="/product_1.png" alt="" />
        <ul>
          <li class="product-C">經典漢堡套餐</li>
          <li class="product-E">Classic Hamburger Package</li>
          <li class="price">
            $
            <span>120</span>
          </li>
          <li class="shopcart">
            <input type="submit" value="加入購物車" />
            <i class="fa fa-shopping-cart" aria-hidden="true" />
          </li>
        </ul>
      </div>
      <div class="product menu-3">
        {#if item5}
          <i class="far fa-heart" aria-hidden="true" on:click={toggleItem5} />
        {:else}
          <i class="fas fa-heart" aria-hidden="true" on:click={toggleItem5} />
        {/if}
        <img src="/product_2.png" alt="" />
        <ul>
          <li class="product-C">英俊香腸</li>
          <li class="product-E">Handsome Sausage</li>
          <li class="price">
            $
            <span>1,024</span>
          </li>
          <li class="shopcart">
            <input type="submit" value="加入購物車" />
            <i class="fa fa-shopping-cart" aria-hidden="true" />
          </li>
        </ul>
      </div>
      <div class="product menu-3">
        {#if item6}
          <i class="far fa-heart" aria-hidden="true" on:click={toggleItem6} />
        {:else}
          <i class="fas fa-heart" aria-hidden="true" on:click={toggleItem6} />
        {/if}
        <img src="/product_3.png" alt="" />
        <ul>
          <li class="product-C">漢堡兄弟</li>
          <li class="product-E">Hamburger Brothers</li>
          <li class="price">
            $
            <span>792</span>
          </li>
          <li class="shopcart">
            <input type="submit" value="加入購物車" />
            <i class="fa fa-shopping-cart" aria-hidden="true" />
          </li>
        </ul>
      </div>
      <div class="product menu-3">
        {#if item7}
          <i class="far fa-heart" aria-hidden="true" on:click={toggleItem7} />
        {:else}
          <i class="fas fa-heart" aria-hidden="true" on:click={toggleItem7} />
        {/if}
        <img src="/product_4.png" alt="" />
        <ul>
          <li class="product-C">完美願望</li>
          <li class="product-E">Drangon Ball Package</li>
          <li class="price">
            $
            <span>999,999</span>
          </li>
          <li class="shopcart">
            <input type="submit" value="加入購物車" />
            <i class="fa fa-shopping-cart" aria-hidden="true" />
          </li>
        </ul>
      </div>
    </div>
  </div>
</div>
