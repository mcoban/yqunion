<template>
  <div id="header">
    <div class="container">
      <a href="/" class="home">
        <img src="../assets/img/logo.png" alt="Logo" height="35">
      </a>
      <a @click="mobileMenuClicked = !mobileMenuClicked" :class="['mobile-menu-button', { clicked: mobileMenuClicked } ]">
        <img src="../assets/img/menu.svg" alt="Mobile Menu" height="24" />
      </a>
      <nav :class="['nav', { visible: mobileMenuClicked }]">
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Products</a></li>
          <li><a href="#">Blog</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data () {
    return {
      mobileMenuClicked: false
    }
  }
}
</script>


<style lang="scss">
@import "../assets/styles/layouts";
#header {
  width: 100%;
  background: #fff;
  padding: 18px 0;
  border-bottom: 1px solid #eee;

  .container {
    display: flex;
    align-items: center;
  }

  .home {
    img {
      display: block;
    }
  }

  .mobile-menu-button {
    position: absolute;
    right: 0;
    padding: 5px 15px;
    display: none;
    transition: ease all .2s;
  }
  
  .nav {
    margin-left: auto;
    ul {
      list-style: none;
      li {
        display: inline;
        margin-left: 40px;
        font-size: 16px;
        font-weight: 500;
        a {
          &:hover {
            color: #007BEB;
          }
        }
      }
    }
  }

  @media screen and (max-width: $mobile) {
    padding: 0;
    .home img {
      padding: 10px 0;
      height: 30px;
    }
    .mobile-menu-button {
      display: flex;
      align-items: center;
      &.clicked {
        transform: rotate(-90deg);
      }
    }
    .nav {
      display: none;
      position: fixed;
      left: 0;
      top: 50px;
      background: #fff;
      z-index: 1;
      width: 100%;
      padding: 30px 0;
      box-sizing: border-box;
      height: calc(100% - 50px);
      border-top: 1px solid #ddd;
      &.visible {
        display: block;
      }
      
      ul {
        li {
          display: block;
          box-sizing: border-box;
          margin: 0;
          a {
            display: block;
            padding: 15px 30px;
            font-size: 21px;
          }
        }
      }
    }
  }
}
</style>
