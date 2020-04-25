<svelte:head>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.13.0/css/all.min.css" integrity="sha256-h20CPZ0QyXlBuAw7A+KluUYx/3pK+c7lYEpqLTlxjYQ=" crossorigin="anonymous" />
  <!-- <link rel="stylesheet" href="font-awesome.min.css" crossorigin="anonymous" /> -->
</svelte:head>

<style>
  .footer {
    width: 100%;
    padding-top: 5%;
    padding-bottom: 5%;
    background-color: #efe9e7;
    overflow: auto;
    font-size: 16px;
  }
  @media (max-width: 414px) {
    .footer {
      padding-top: 10%;
      padding-bottom: 10%;
    }
  }
  .footer > div {
    float: left;
  }
  .footer .about {
    width: 28.33333%;
    padding-left: 5%;
  }
  @media (max-width: 414px) {
    .footer .about {
      width: 95%;
      margin-bottom: 30px;
    }
  }
  .footer .about span {
    font-size: 24px;
  }
  .footer .about p {
    margin-top: 20px;
    line-height: 20px;
  }
  .footer .contact {
    width: 29.33333%;
    padding-left: 4%;
  }
  @media (max-width: 414px) {
    .footer .contact {
      width: 96%;
      margin-bottom: 20px;
    }
  }
  .footer .contact span {
    font-size: 24px;
  }
  .footer .contact ul {
    margin-top: 20px;
  }
  @media (max-width: 414px) {
    .footer .contact ul {
      padding-left: 6%;
    }
  }
  .footer .contact ul li {
    margin-bottom: 8px;
    list-style-type: disc;
  }
  .footer .contact ul li a {
    color: #3d1101;
  }
  .footer .link {
    float: right;
    padding-right: 5%;
  }
  .footer .link img {
    margin-top: 10px;
    margin-bottom: 20px;
  }
  .footer .link ul {
    text-align: right;
  }
  .footer .link ul li {
    display: inline;
    font-size: 40px;
    margin-left: 10px;
  }
  .footer .link .google {
    color: #ff5151;
  }
  .footer .link .twitter {
    color: #46a3ff;
  }
  .footer .link .facebook {
    color: #004b97;
  }
</style>

<div class="footer">
  <div class="about">
    <span>關於六角西餐廳</span>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Similique
      reiciendis earum, consectetur beatae repellendus doloribus voluptates quas
      est ducimus obcaecati incidunt quos quo, illo in.
    </p>
  </div>
  <div class="contact">
    <span>聯絡方式</span>
    <ul>
      <li>高雄市中正五路到底</li>
      <li>+886 886 886</li>
      <li>
        <a href="#/">service@hexschool.com</a>
      </li>
    </ul>
  </div>
  <div class="link">
    <img src="/logo_l(null).svg" alt="" />
    <ul>
      <li>
        <a href="#/">
          <i class="fab fa-google-plus-square google" aria-hidden="true" />
        </a>
      </li>
      <li>
        <a href="#/">
          <i class="fab fa-twitter-square twitter" aria-hidden="true" />
        </a>
      </li>
      <li>
        <a href="#/">
          <i class="fab fa-facebook-square facebook" aria-hidden="true" />
        </a>
      </li>
    </ul>
  </div>
</div>

