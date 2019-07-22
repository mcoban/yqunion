<template>
  <Layout>
    <div class="hero">
      <div class="container">
        <div class="content-section">
          <h1>WE ARE THE BEST AT THE INDUSTRY</h1>
          <h2>Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat deleniti impedit</h2>
          <a class="btn content-section__product">View Our Products</a>
        </div>
      </div>
      <div class="main-products">
        <a class="product product-1">
          <span class="title">Cable System</span>
        </a>
        <a class="product product-2">
          <span class="title">Battery System</span>
        </a>
        <a class="product product-3">
          <span class="title">Lighting System</span>
        </a>
        <a class="product product-4">
          <span class="title">Industrial System</span>
        </a>
      </div>
    </div>
    <section class="section pt_70">
      <div class="container center narrow">
        <h4 class="section__title">WHAT MAKES US SPECIAL</h4>
        <h3 class="section__big_text">
          The Metropolitan Museum of Art is banning selfie sticks
        </h3>
      </div>
    </section>
    
    <section class="section interactive-map">
      <div class="container">
        <img class="map" src="../assets/img/map.png" alt="Interactive Map">
      </div>
    </section>

    <section class="section content_1">
      <div class="white">
        <g-image src="../assets/img/content_1.jpg" fit="cover" alt="Conten1" />
      </div>
      <div class="blue">
        <span class="title">Collaborate with your team and design in real-time</span>
        <span class="subtitle">In the tumultuous business of cutting-in and attending to a whale, there is much running backwards and forwards among the crew.</span>
        <a href="#" class="discover">Discover</a>
      </div>
    </section>

    <section class="section news">
      <div class="container">
        <h3 class="section__blue_title">News from Us</h3>
        <div class="grid news mt_40">
          <div class="card span_4">
            <img src="../assets/img/card-image-1.png" alt="card image 1">
            <div class="info p_30">
              <span class="card__title">Card 1</span>
              <span class="card__description mt_10">Being the savage's bowsman</span>
            </div>
          </div>
          <div class="card span_4">
            <img src="../assets/img/card-image-1.png" alt="card image 1">
            <div class="info p_30">
              <span class="card__title">Card 1</span>
              <span class="card__description mt_10">Being the savage's bowsman</span>
            </div>
          </div>
          <div class="card span_4">
            <img src="../assets/img/card-image-1.png" alt="card image 1">
            <div class="info p_30">
              <span class="card__title">Card 1</span>
              <span class="card__description mt_10">Being the savage's bowsman</span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="section mapbox">
      <div class="mapouter">
        <div class="gmap_canvas">
          <iframe width="600" height="500" id="gmap_canvas" src="https://maps.google.com/maps?q=Liushi%2CYueqing%2CZhejiang%2CChina&t=&z=13&ie=UTF8&iwloc=&output=embed" frameborder="0" scrolling="no" marginheight="0" marginwidth="0"></iframe>
          <a href="https://www.embedgooglemap.org"></a>
        </div>
      </div>
      <div class="locations">
        <a href="#" class="location">istanbul</a>
        <a href="#" class="location">bejing</a>
        <a href="#" class="location">sydney</a>
        <a href="#" class="location">new york</a>
      </div>
    </section>

    <section class="section address">
      <div class="container grid">
        <span class="span_5">
          <span class="span__title">Address</span>
          <span class="span__desc">Add:6 Floor,A Building,Hongbao Mansion,No.198-208 Chezhan Road, Liushi, Yueqing, Zhejiang,China</span>
        </span>
        <span class="span_2">
          <span class="span__title">Email</span>
          <span class="span__desc">info@yqunion.com</span>
        </span>
        <span class="span_3">
          <span class="span__title">Phone</span>
          <span class="span__desc">+86-577-61780552</span>
        </span>
        <span class="span_2">
          <a href="#" class="contact">contact us</a>
        </span>
      </div>
    </section>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Hello, world!'
  }
}
</script>

<style lang="scss">
.hero {
  width: 100%;
  height: 700px;
  background: url(../assets/img/hero.jpg) center center no-repeat;
  position: relative;
  background-size: cover;

  .content-section {
    padding-top: 160px;
    max-width: 600px;

    h1 {
      color: #fff;
      font-size: 60px;
      font-weight: 800;
      line-height: 1.3;
      text-shadow: 0 2px 10px rgba(0,0,0,0.20);
    }

    h2 {
      font-weight: 400;
      font-size: 22px;
      color: #fff;
      letter-spacing: 0.6px;
      margin-top: 10px;
    }
  }

  .main-products {
    position: absolute;
    width: 720px;
    height: 160px;
    grid-gap: 5px;
    bottom: -80px;
    left: calc(50% - 360px);
    display: grid;
    grid-template: 1fr / repeat(4, 1fr);
    overflow: hidden;

    a {
      padding: 20px;
      cursor: pointer;
      transition: ease all .2s;
      position: relative;

      .title {
        position: absolute;
        bottom: 20px;
        font-size: 16px;
        font-weight: 500;
      }

      &:hover {
        .title {
          color: #fff;
        }
      }

      &.product-1 {
        background: url(../assets/img/plug.svg) 20px 20px no-repeat #f1f1f1;
        background-size: 48px;
        &:hover {
          background: url(../assets/img/plug-white.svg) 20px 20px no-repeat #181A82;
          background-size: 48px;
        }
      }
      &.product-2 {
        background: url(../assets/img/battery.svg) 20px 20px no-repeat #f1f1f1;
        background-size: 48px;
        &:hover {
          background: url(../assets/img/battery-white.svg) 20px 20px no-repeat #181A82;
          background-size: 48px;
        }
      }
      &.product-3 {
        background: url(../assets/img/chandelier.svg) 20px 20px no-repeat #f1f1f1;
        background-size: 48px;
        &:hover {
          background: url(../assets/img/chandelier-white.svg) 20px 20px no-repeat #181A82;
          background-size: 48px;
        }
      }
      &.product-4 {
        background: url(../assets/img/electric-pole.svg) 20px 20px no-repeat #f1f1f1;
        background-size: 48px;
        &:hover {
          background: url(../assets/img/electric-pole-white.svg) 20px 20px no-repeat #181A82;
          background-size: 48px;
        }
      }
    }
  }

}
.interactive-map {
  text-align: center;
  .map {
    width: 100%;
    max-width: 1000px;
  }
}

.content_1 {
  height: 920px;
  display: grid;
  grid-template: 1fr / 1fr 1fr;

  .white {
    background: #fff;
    display: flex;
    align-items: center;
    img {
      width: 110%;
      z-index: 1;
    }
  }

  .blue {
    background: #181A82;
    box-sizing: border-box;
    padding: 120px;


    .title {
      margin-left: 50px;
      font-weight: 400;
      font-size: 40px;
      color: #fff;
      letter-spacing: 0.29px;
      text-align: left;
      margin-top: 200px;
      display: block;
    }

    .subtitle {
      font-weight: 300;
      font-size: 18px;
      color: #fff;
      letter-spacing: 0.17px;
      text-align: left;
      display: block;
      line-height: 27.67px;
      margin-left: 50px;
    }

    .discover {
      padding: 15px 40px;
      color: #fff;
      background: #00C3FF;
      margin: 30px 50px;
      display: inline-block;
    }
  }
}

.btn {
  background: #eee;
  padding: 18px 15px 15px;
  font-size: 16px;
  line-height: 16px;
  font-weight: 500;
  display: inline-block;
  cursor: pointer;

  &.content-section__product {
    margin-top: 50px;
    color: #fff;
    background: #181A82;
    border-radius: 40px;
    padding-left: 30px;
    padding-right: 30px;
    margin-top: 20px;
  }
}

.news {
  .card {
    img {
      width: 100%;
    }

    .card__title {
      font-weight: 400;
      font-size: 22px;
      color: #00C3FF;
      letter-spacing: 0.15px;
      display: block;
    }
    .card__description {
      font-size: 17px;
      font-display: 400;
      display: block;
    }
  }
}

.mapbox {
  border-bottom: 1px solid #eee;
  .map {
    background: #eee;
    height: 600px;
    margin-bottom: 50px;
  }
  .gmap_canvas {
    margin-bottom: 50px;
    iframe {
      width: 100%;
    }
  }

  .locations {
    width: 400px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    padding-bottom: 50px;

    .location {
      font-weight: 700;
      text-transform: uppercase;
      font-size: 14px;
      color: #989898;
      letter-spacing: 0.58px;
    }
  }
}

.address {
  margin: 0;
  padding: 50px 0;
  border-bottom: 1px solid #eee;

  .span__title {
    font-weight: 500;
    font-size: 19px;
    color: #323C47;
    letter-spacing: 0;
    display: block;
  }

  .span__desc {
    font-weight: 400;
    font-size: 16px;
    color: #989898;
    letter-spacing: 0;
    line-height: 30.88px;
  }

  .contact {
    background: #4DA1FF;
    padding: 18px 25px 15px 25px;
    text-transform: uppercase;
    font-size: 15px;
    font-weight: 600;
    border-radius: 4px;
    color: #fff;
    &:hover {
      background: darken(#4DA1FF, 10%);
    }
  }
}

</style>


<script>
export default {
  metaInfo: {
    title: 'Yqunion'
  }
}
</script>