<style>
  .login {
    width: 360px;
    margin: 0 auto;
    padding-top: 5%;
    color: #3d1101;
    padding-bottom: 5%;
  }
  @media (max-width: 414px) {
    .login {
      width: 90%;
      padding-left: 5%;
      padding-right: 5%;
    }
  }
  .login > div {
    text-align: center;
    margin-bottom: 40px;
  }
  .login > div h2 {
    font-size: 20px;
    font-weight: bold;
    margin-top: 10px;
  }
  .login form {
    padding-left: 4%;
    padding-right: 4%;
    padding-bottom: 6%;
    overflow: auto;
    box-shadow: 9px 4px 11px rgba(10, 10, 10, 0.1);
    border: 1px solid #d0d0d0;
    border-top: 3px solid #f75000;
    position: relative;
  }
  @media (max-width: 414px) {
    .login form {
      padding-left: 0;
      padding-right: 0;
    }
  }
  .login form span {
    width: 100%;
    float: left;
    margin-top: 20px;
    margin-bottom: 5px;
  }
  .login form span:first-child {
    text-align: center;
    font-weight: bold;
    font-size: 18px;
  }
  .login form .forget {
    color: #f75000;
    float: left;
    margin-top: 5px;
    font-size: 14px;
  }
  .login form .login-data {
    background: #fff;
    height: 32px;
    width: 100%;
    position: relative;
    margin-top: 10px;
  }
  .login form .login-data input[type="text"] {
    border: 0px;
    height: 30px;
    float: right;
    width: 97%;
    padding-left: 3%;
  }
  .login form .login-data i {
    position: absolute;
    left: 10px;
    font-size: 20px;
    top: 5px;
    color: gray;
  }
  .login form > div {
    width: 100%;
    float: left;
    text-align: center;
    margin-top: 40px;
  }
  .login form > div input[type="submit"] {
    display: inline-block;
    width: 45%;
    padding: 8px 0;
    color: #fff;
    border: 0px;
    border-radius: 3px;
  }
  .login form > div .gotoRegister {
    background: gray;
    float: left;
    width: 45%;
    padding: 4px 0;
    color: #fff;
    border: 0px;
    border-radius: 3px;
  }
  .login form > div .gotoLogin {
    background: #f75000;
    float: right;
  }
  a {
    text-decoration: none;
  }
</style>

<svelte:head>
  <title>Login</title>
</svelte:head>

<div class="login">
  <div>
    <img src="images/logo_l(null).svg" alt="" />
    <h2>享受美食好味道</h2>
  </div>
  <form action="#">
    <span>LOGIN</span>
    <span>Email Address*</span>
    <div class="login-data">
      <input type="text" />
      <i class="fa fa-envelope" aria-hidden="true" />
    </div>
    <span>Password*</span>
    <div class="login-data">
      <input type="text" />
      <i class="fa fa-lock" aria-hidden="true" />
    </div>
    <a class="forget" href="#/">忘記密碼?</a>
    <div>
      <a class="gotoRegister" href="/register">註冊</a>
      <input class="gotoLogin" type="submit" value="登入" />
    </div>
  </form>
</div>
