<style>
  .feature {
    width: 100%;
    padding-top: 5%;
    padding-bottom: 5%;
    overflow: auto;
    overflow-x: hidden;
  }
  @media (max-width: 414px) {
    .feature {
      padding-top: 10%;
    }
  }
  .feature > div {
    overflow: auto;
    margin-bottom: 30px;
    position: relative;
  }
  .feature > div::before {
    position: absolute;
    content: " ";
    border-bottom: 1px solid #d0d0d0;
    height: 5px;
    width: 14%;
    top: 18px;
    left: 25%;
  }
  @media (max-width: 414px) {
    .feature > div::before {
      display: none;
    }
  }
  .feature > div::after {
    position: absolute;
    content: " ";
    border-bottom: 1px solid #d0d0d0;
    height: 5px;
    width: 14%;
    top: 18px;
    right: 25%;
  }
  @media (max-width: 414px) {
    .feature > div::after {
      display: none;
    }
  }
  .feature span {
    font-size: 20px;
    width: 100%;
    float: left;
    text-align: center;
    margin-bottom: 10px;
  }
  .feature ul {
    width: 90%;
    margin: 20px 5% 0 5%;
  }
  .feature ul li {
    display: inline-block;
    width: 30.33333%;
    float: left;
    text-align: center;
    margin-right: 4.5%;
    font-size: 18px;
  }
  @media (max-width: 414px) {
    .feature ul li {
      width: 90%;
      padding-left: 5%;
      padding-right: 5%;
      margin-bottom: 10%;
    }
  }
  .feature ul li img {
    border-radius: 100px;
    margin-bottom: 20px;
  }
  .feature ul li span {
    margin-bottom: 20px;
    font-size: 18px;
  }
  .feature ul li p {
    font-size: 18px;
  }
  .feature ul li:last-child {
    margin-right: 0;
  }

  .chief {
    width: 100%;
    overflow: auto;
    background-color: #3d1101;
    color: #fff;
    height: auto;
    overflow-y: hidden;
  }
  .chief .chief-img {
    width: 45%;
    margin-left: 42px;
    height: 460px;
    float: left;
    background-position: center center;
  }
  @media (max-width: 768px) {
    .chief .chief-img {
      margin-left: 20px;
    }
  }
  @media (max-width: 414px) {
    .chief .chief-img {
      width: 100%;
      margin-left: 0;
      background-position: 100% center;
    }
  }
  .chief .chief-today {
    float: right;
    width: 40%;
    padding: 10% 7% 0 0;
    line-height: 20px;
    font-size: 16px;
  }
  @media (max-width: 768px) {
    .chief .chief-today {
      padding: 5% 5% 0 0;
    }
  }
  @media (max-width: 414px) {
    .chief .chief-today {
      width: 80%;
      padding: 10%;
    }
  }
  .chief .chief-today .chief-name {
    width: 100%;
    font-size: 20px;
    float: left;
    line-height: 25px;
    margin-bottom: 15px;
  }
  .chief .chief-today .chief-name:first-child {
    margin-bottom: 0px;
  }
  .chief .chief-today .chief-name:first-child span {
    margin-left: 10px;
    margin-right: 10px;
  }

  .avatar {
    width: 100%;
    overflow: auto;
    margin-bottom: 5%;
  }
  .avatar > div {
    text-align: center;
    margin-top: 5%;
    margin-bottom: 5%;
    font-size: 24px;
  }
  @media (max-width: 414px) {
    .avatar > div {
      margin-top: 10%;
    }
  }
  .avatar ul {
    width: 90%;
    margin: 0 5% 0 5%;
  }
  .avatar ul li {
    display: inline-block;
    width: 33.33333%;
    float: left;
  }
  @media (max-width: 414px) {
    .avatar ul li {
      width: 100%;
    }
  }
  .avatar ul li img {
    border-radius: 100px;
    width: 20%;
    float: left;
  }
  .avatar ul li .impression {
    width: 70%;
    float: right;
    padding-right: 7%;
    padding-left: 3%;
  }
  @media (max-width: 414px) {
    .avatar ul li .impression {
      width: 77%;
      padding-right: 0;
    }
  }
  .avatar ul li .impression span {
    width: 100%;
    float: left;
    margin-bottom: 25px;
    font-size: 16px;
  }
  .avatar ul li .impression span:last-child {
    text-align: right;
  }

  .map {
    background-color: #fffafa;
    overflow: auto;
    padding: 0 5% 5% 5%;
  }
  .map .map-title {
    margin-top: 5%;
    margin-bottom: 5%;
    font-size: 24px;
    overflow: auto;
    overflow-y: hidden;
  }
  @media (max-width: 414px) {
    .map .map-title {
      margin-top: 10%;
    }
  }
  .map .map-title span {
    width: 100%;
    float: left;
    line-height: 30px;
    text-align: center;
  }
  .map .tinymap {
    height: 386px;
    width: 50%;
    float: left;
    border: 1px solid #d0d0d0;
  }
  @media (max-width: 414px) {
    .map .tinymap {
      width: 100%;
    }
  }
  .map form {
    float: right;
    height: 386px;
    width: 45%;
    position: relative;
  }
  @media (max-width: 414px) {
    .map form {
      width: 100%;
      margin-top: 10%;
    }
  }
  .map form span {
    width: 100%;
    float: left;
    font-size: 14px;
    margin-bottom: 10px;
  }
  .map form input[type="text"] {
    width: 95%;
    float: left;
    margin-bottom: 15px;
    border-style: none;
    border: 1px solid #d0d0d0;
    border-radius: 3px;
    height: 28px;
    padding-left: 10px;
  }
  .map form input[type="radio"] {
    width: 16px;
    height: 16px;
    vertical-align: middle;
    margin: 0;
    margin-right: 35px;
  }
  .map form input[type="radio"]:hover {
    border-color: blue;
  }
  .map form input[type="radio"]::before {
    content: " ";
    display: block;
    width: 60%;
    height: 60%;
    margin: 17.5% 17.5%;
    border-radius: 50%;
  }
  .map form input[type="radio"]:checked:before {
    background: #66b3ff;
  }
  .map form .sent-form {
    position: absolute;
    bottom: 0;
    right: 10px;
    font-family: "PingFangTC-Regular";
  }
  .map form .sent-form a {
    padding: 5px 15px;
    border-radius: 4px;
    color: #fff;
    font-size: 14px;
  }
  .map form .sent-form .cancel {
    background-color: gray;
  }
  .map form .sent-form .sent {
    background-color: #ff5809;
    margin-left: 15px;
  }
</style>

<div class="feature">
  <div>
    <span>客人總是在詢問</span>
    <span>這麼好吃的秘訣是什麼</span>
  </div>
  <ul>
    <li>
      <img src="/feature_1.png" alt="" />
      <span>台灣本土蔬菜</span>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nulla est
        perferendis expedita, sed a quaerat quis facilis dolor laborum id
        accusantium sit neque quas qui, officia reprehenderit eum voluptas!
        Placeat quos ab voluptas quod, aliquam molestias
      </p>
    </li>
    <li>
      <img src="/feature_2.png" alt="" />
      <span>專業米其林廚師</span>
      <p>
        architecto, minima. Molestiae sint, accusantium ipsa officia culpa
        doloribus, hic assumenda autem illum corporis impedit officiis animi
        aut! Minus cupiditate, soluta itaque. Quae unde doloremque
      </p>
    </li>
    <li>
      <img src="/feature_3.png" alt="" />
      <span>對於專業不能退讓</span>
      <p>
        adipisci nemo ex, cupiditate recusandae magni qui dolores odio saepe!
        Ea, cumque, praesentium ratione tempore placeat consequatur maxime
        incidunt quasi nobis suscipit nulla cum velit fuga quia error? Est
        quidem recusandae incidunt distinctio, voluptatem tenetur possimus
        illum, deserunt vero?
      </p>
    </li>
  </ul>
</div>
<div class="chief">
  <div class="chief-img" style="background-image: url(/main_chef_brown.png);" />
  <div class="chief-today">
    <span class="chief-name">
      今日主廚
      <span>:</span>
      金森、梅在帕
    </span>
    <span class="chief-name">
      Today Chief
      <span>:</span>
      Plum in Shock
    </span>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Provident culpa
      atque eos ullam. At molestias ea rem, repudiandae omnis, delectus eaque
      asperiores sequi quaerat debitis obcaecati fugit nisi numquam quod ullam
      fuga dolorem inventore veniam cupiditate voluptatibus consectetur
      temporibus id voluptatum. Hic accusantium delectus, perspiciatis assumenda
      dignissimos incidunt ab alias!
    </p>
  </div>
</div>
<div class="avatar">
  <div>聽聽別人的感想</div>
  <ul>
    <li>
      <img src="/avatar_1.png" alt="" />
      <div class="impression">
        <span>高雄吃一口</span>
        <span>
          自從吃了這家餐廳後，我口水流了一個多月沒停，下次不要再被我遇到，我然我一定連他們的桌子一起啃下去。
        </span>
        <span>--產品經理</span>
      </div>
    </li>
    <li>
      <img src="/avatar_2.png" alt="" />
      <div class="impression">
        <span>廟口小霸王</span>
        <span>
          自從吃了這家餐廳後，我口水流了一個多月沒停，下次不要再被我遇到，我然我一定連他們的桌子一起啃下去。
        </span>
        <span>--金身道士</span>
      </div>
    </li>
    <li>
      <img src="/avatar_3.png" alt="" />
      <div class="impression">
        <span>春天來了</span>
        <span>
          自從吃了這家餐廳後，我口水流了一個多月沒停，下次不要再被我遇到，我然我一定連他們的桌子一起啃下去。
        </span>
        <span>--美麗萬分</span>
      </div>
    </li>
  </ul>
</div>
<div class="map">
  <div class="map-title">
    <span>我們的位置不太夠坐</span>
    <span>要不要先定位呢？</span>
  </div>
  <div class="tinymap" />
  <form action="">
    <span>姓名</span>
    <input type="text" />
    <span>電話</span>
    <input type="text" />
    <span>信箱</span>
    <input type="text" />
    <span>人數</span>
    <input type="text" />
    <span>是否需要素食</span>
    <span>
      是
      <input type="radio" name="vegetable" value="need" />
      否
      <input type="radio" name="vegetable" value="notneed" />
    </span>
    <div class="sent-form">
      <a href="#/" class="cancel">取消</a>
      <a href="#/" class="sent">送出</a>
    </div>
  </form>
</div>
