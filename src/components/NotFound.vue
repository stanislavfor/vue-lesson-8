<template>
  <div class="container">
    <div class="content">
      <h2 class="error-code">404</h2>
      <p class="error-message">
        Приносим извинения, но страница,<br>
        которую вы искали,<br>
        не найдена
      </p>
      <router-link to="/" class="home-button">Домой</router-link>
    </div>
    <div class="image-container">
      <img src="@/assets/images/img-404.png" alt="image-for-page-404" class="image">
    </div>
  </div>
</template>

<script>
export default {
  name: 'NotFound'
}
</script>

<style scoped>
body {
  font-family: Lobster, cursive;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: #f5f5f5;
}
.container {
  width: 1201px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.content {
  text-align: center;
  width: 50%;
}
.error-code {
  font-size: 150px;
  color: #cd7f32;
  margin: 0;
}
.error-message {
  font-size: 24px;
  color: #333;
  margin: 20px 0;
  margin-bottom: 100px;
}
.home-button {
  cursor: pointer;
  text-decoration: none;
  color: #fff;
  display: inline-block;
  font-weight: 400;
  font-family: Jost, sans-serif;
  font-size: 18px;
  line-height: 27px;
  letter-spacing: .72px;
  background-color: #292f36;
  padding: 22px 67px 22px 34px;
  border-radius: 18px;
  position: relative;
  -webkit-transition: text-shadow .3s;
  -o-transition: text-shadow .3s;
  transition: text-shadow .3s;
}
.home-button::before {
  content: "";
  width: 29px;
  height: 36px;
  background-image: url(@/assets/images/contact-arrow-brown.svg);
  background-repeat: no-repeat;
  position: absolute;
  background-size: contain;
  right: 20px;
  top: 50%;
  -webkit-transform: translateY(-50%);
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
}
.home-button:hover {
  background-color: #555;
}
.image-container {
  width: 50%;
  position: relative;
}
.image {
  width: 100%;
  height: auto;
  right: 0;
}
</style>
