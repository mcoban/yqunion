<template>
  <div id="header">
    <div class="container">
      <a href="/" class="home">
        <img src="../assets/img/logo.png" alt="Logo" height="35">
      </a>
      <nav class="nav">
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


<style lang="scss">
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
}
</style>
