<template>
  <footer class="section">
    <div class="container grid">
      <a href="#" class="span_3">
        <img src="../assets/img/logo.png" alt="Logo" width="150" />
      </a>
      <div class="span_2">
        <h4>Services</h4>
        <ul>
          <li><a href="#">Popular</a></li>
          <li><a href="#">Trending</a></li>
          <li><a href="#">Catalog</a></li>
        </ul>
      </div>
      <div class="span_2">
        <h4>Product</h4>
        <ul>
          <li><a href="#">Popular</a></li>
          <li><a href="#">Trending</a></li>
          <li><a href="#">Catalog</a></li>
        </ul>
      </div>
      <div class="span_3">
        <h4>Info</h4>
        <ul>
          <li><a href="#">Popular</a></li>
          <li><a href="#">Trending</a></li>
          <li><a href="#">Catalog</a></li>
        </ul>
      </div>
      <div class="span_2">
        <h4>follow us</h4>
        <a class="social" target="_blank" rel="nofollow" href="#"><img src="../assets/img/facebook.png" alt="Facebook" height="20"></a>
        <a class="social" target="_blank" rel="nofollow" href="#"><img src="../assets/img/twitter.png" alt="Twitter" height="20"></a>
        <a class="social" target="_blank" rel="nofollow" href="#"><img src="../assets/img/instagram.png" alt="Instagram" height="20"></a>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
.section {
  margin: 50px 0;
}

h4 {
  font-size: 16px;
  margin-bottom: 20px;
  text-transform: uppercase;
  font-weight: 600;
}
li {
  list-style: none;
  margin-bottom: 5px;
  a {
    color: #777;
    font-size: 15px;
  }
}
.social {
  margin-right: 15px;
}
</style>
