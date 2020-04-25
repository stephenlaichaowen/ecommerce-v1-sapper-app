<style>
  .register {
    width: 60%;
    margin: auto;
    padding-top: 5%;
    color: #3d1101;
    padding-bottom: 5%;
  }
  @media (max-width: 414px) {
    .register {
      width: 100%;
    }
  }
  .register > div {
    text-align: center;
    margin-bottom: 40px;
  }
  .register > div h2 {
    font-size: 20px;
    font-weight: bold;
    margin-top: 10px;
  }
  .register span {
    width: 100%;
    float: left;
    margin-top: 20px;
    margin-bottom: 5px;
  }
  .register .register-title {
    text-align: center;
    font-weight: bold;
    font-size: 18px;
  }
  .register form {
    padding-left: 4%;
    padding-right: 4%;
    padding-bottom: 3%;
    overflow: auto;
    box-shadow: 9px 4px 11px rgba(10, 10, 10, 0.1);
    border: 1px solid #d0d0d0;
    border-top: 3px solid #f75000;
    position: relative;
  }
  .register .rule {
    width: 50%;
    float: left;
    line-height: 20px;
  }
  .register .rule span {
    font-size: 18px;
  }
  .register .register-form {
    width: 48%;
    float: right;
    margin-left: 2%;
  }
  .register .register-form .register-data {
    background: #fff;
    height: 32px;
    width: 100%;
    position: relative;
    float: left;
  }
  .register .register-form .register-data input[type="text"] {
    border: 0px;
    height: 30px;
    float: right;
    width: 97%;
    padding-left: 3%;
  }
  .register .register-form .register-data i {
    position: absolute;
    left: 10px;
    font-size: 20px;
    top: 5px;
    color: gray;
  }
  .register .register-form .checkagain {
    margin-top: 10px;
  }
  .register .register-form .already {
    color: #f75000;
    float: left;
    margin-top: 5px;
    font-size: 14px;
  }
  .register .register-form .register-sent {
    width: 100%;
    float: left;
    text-align: right;
    margin-top: 10%;
  }
  .register .register-form .register-sent input[type="submit"] {
    background: #f75000;
    width: 45%;
    padding: 8px 0;
    color: #fff;
    border: 0px;
    border-radius: 3px;
  }
</style>

<svelte:head>
  <title>Register</title>
</svelte:head>

<div class="register">
  <div>
    <img src="/logo_l(null).svg" alt="" />
    <h2>享受美食好味道</h2>
  </div>
  <form action="#">
    <span class="register-title">REGISTER</span>
    <div class="rule">
      <span>就是這樣條款 :</span>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae
        quae possimus suscipit non voluptatibus veniam quia voluptatum quidem,
        sit adipisci.
      </p>
    </div>
    <div class="register-form">
      <span>Email Address*</span>
      <div class="register-data">
        <input type="text" />
        <i class="fa fa-envelope" aria-hidden="true" />
      </div>
      <span>Password*</span>
      <div class="register-data">
        <input type="text" />
        <i class="fa fa-lock" aria-hidden="true" />
      </div>
      <div class="register-data checkagain">
        <input type="text" />
        <i class="fa fa-lock" aria-hidden="true" />
      </div>
      <a class="already" href="#/">已經有帳號了?</a>
      <div class="register-sent">
        <a href="/register">
          <input class="gotoRegister" type="submit" value="註冊" />
        </a>
      </div>
    </div>
  </form>
</div>
