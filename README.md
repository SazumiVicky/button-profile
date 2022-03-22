# Button Profile Open Source

## &#x270d; HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Sazumi Viki Button Css - Html</title>
    <meta property="og:description" content="Sazumi Viki Button Html - Css">
    <meta property="og:site_name" content="Sazumi Viki">
    <meta content='Sazumi Viki Button Html - Css' property='og:description' />
    <link rel="alternate icon" class=js-site-favicon type=image/ico href=https://dev.sazumiviki.com/favku>
    <link rel=icon class=js-site-favicon type=image/ico+xml href=https://dev.sazumiviki.com/favku>
    <link rel="stylesheet" href="style.css">
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <ion-content has-header="true">
        <div id="profile-bg"></div>
        <div id="content">
          <div id="profile-info">
            <img id="profile-image" src="https://cdn.jsdelivr.net/gh/SazumiVicky/sazumi.developer@main/gawr-gura-sazumi.jpg">
            <h3 id="profile-name">Sazumi Viki</h3>
            <span id="profile-description">Front End Development Of <a href="https:sazumiviki.com">Sazumi Viki</a>, Developer Of
              <a href="https://sazumiviki.com">Sazumi Viki</a></span>
          </div>
    <title>Document</title>
</head>
<body>
        <div class="button_container">
            <div class="sazumi_btn">
              <span class="su_button_circle">
              </span>
              <a href="https://www.sazumiviki.com" class="sazumi_btn_inner">
                <span class="button_text_container">
                  Button 1
                </span>
              </a>
            </div>
      
            <div class="sazumi_btn">
              <span class="su_button_circle">
              </span>
              <a href="https://www.sazumiviki.com" class="sazumi_btn_inner">
                <span class="button_text_container">
                  Button 2
                </span>
              </a>
            </div>
      
            <div class="sazumi_btn">
              <span class="su_button_circle">
              </span>
              <a href="https://www.sazumiviki.com" class="sazumi_btn_inner">
                <span class="button_text_container">
                  Button 3
                </span>
              </a>
            </div>
      
            <div class="sazumi_btn">
              <span class="su_button_circle">
              </span>
              <a href="https://www.sazumiviki.com" class="sazumi_btn_inner">
                <span class="button_text_container">
                  Button 4
                </span>
              </a>
            </div>
        </div>
        <p class="credit">Tekhnologi Oleh <b>Sazumi</b></p>
      </div>
</body>
</html>
```

## &#x270d; CSS

```css
@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');

body {
  font-family: 'Lato', sans-serif;
  background: #ffffff;
}

h1{
  text-align: center;
  color: #215c7a;
}

.credit{
  text-align: center;
  color: #215c7a;

}

.content{
  padding-top: 45px;
  padding-bottom: 20px;
}

.button_container{
    width: 176px;
    margin: 0 auto;
    margin-top: initial;
    padding-top: 40px;
}

.sazumi_btn{
  overflow: hidden;
  position: relative;
  display: inline-block;
  border-radius: 3px;
  margin-bottom: 30px;
}

.su_button_circle{
  background-color: red;
  border-radius: 1000px;
  position: absolute;
  left:0;
  top:0;
  width: 0px;
  height: 0px;
  margin-left: 0px;
  margin-top: 0px;
  pointer-events: none;
  /*animation-timing-function: ease-in-out; */
}

.sazumi_btn_inner{
    display: inline-block;
    background: #215c7a;
    color: #F4F4F4;
    font-size: 16px;
    font-weight: normal;
    width: 132px;
    text-align: center;
    border-radius: 3px;
    transition: 400ms;
    text-decoration: none;
    padding: 22px;
    z-index: 100000;
}

.button_text_container{
   position:relative;
   z-index: 10000;
}

.explode-circle {
   animation: explode 0.5s forwards;

}

.desplode-circle{
   animation: desplode 0.5s forwards;
}

@keyframes explode {
  0% {
    width: 0px;
    height: 0px;
    margin-left: 0px;
    margin-top: 0px;
    background-color: rgba(42, 53, 80,0.2);
  }
  100% {
    width: 400px;
    height: 400px;
    margin-left: -200px;
    margin-top: -200px;
    background-color: rgba(20, 180, 87,0.8);
  }
}

@keyframes desplode {
  0% {
    width: 400px;
    height: 400px;
    margin-left: -200px;
    margin-top: -200px;
    background-color: rgba(20, 180, 87,0.8);
  }
  100% {
    width: 0px;
    height: 0px;
    margin-left: 0px;
    margin-top: 0px;
    background-color: rgba(129, 80, 108,0.6);
  }
}
/* Profile Css */
#profile-bg {
    position: fixed;
    left: 0;
    top: 44px;
    width: 100%;
    height: 150px;

/*     background: url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/94311/bg.jpg') no-repeat transparent;*/
    background-size: 100%;
    background-position: 50% 20%;

    text-align: center;
  }

  #content {
    position: relative;
    margin-top: 150px;
    padding-top: 200px;
  }

  #profile-info {
    position: absolute;
    top: -95px;
    width: 100%;
    z-index: 2;
    text-align: center;
  }
  #profile-name {
    color: #444;
    font-size: 26px;
  }
  #profile-description {
    font-size: 15px;
    color: #888;
  }
  #profile-description a {
    color: #888;
  }

  #profile-image {
    display: block;
    border-radius: 100px;
    border: 1px solid #fff;
    width: 128px;
    height: 128px;
    margin: 10px auto 0;
    box-shadow: 0px 0px 4px rgb(195 160 160 / 70%);
  }

  .list-item-content {
    padding: 5px;
  }

  .list-item {
    color: #666666;
  }

  .post {
    color: #444;
  }

  .post-time {
    position: absolute;
    right: 5px;
    top: 5px;
    font-size: 11px;
    color: #888;
  }

  .post-profile-image {
    display: inline-block;
    vertical-align: top;
    width: 48px;
    height: 48px;
    margin-right: 10px;
  }
  .post-options {
    position: absolute;
    font-size: 16px;
    right: 5px;
    bottom: 5px;
    color: #888;
  }
```
