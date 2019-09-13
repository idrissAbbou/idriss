<template>
  <div class="tech">
    <div class="container">
      <div class="row tekciy d-flex justify-content-center align-items-center p-4">
        <div class="col-12 d-flex justify-content-between first-row">
          <i class="fab fa-html5"></i>
          <i class="fab fa-css3-alt"></i>
          <i class="fab fa-bootstrap"></i>
          <i class="fab devicon-sass-original"></i>
          <i class="fab fa-js-square"></i>
          <i class="fab fa-vuejs"></i>
        </div>
        <div class="col-12 d-flex justify-content-between second-row">
          <i class="fab devicon-webpack-plain"></i>
          <i class="fab devicon-babel-plain"></i>
          <i class="fab fa-php"></i>
          <i class="fab fa-laravel"></i>
          <i class="fab devicon-wordpress-plain"></i>
          <i class="fab devicon-mysql-plain"></i>
        </div>
        <div class="col-12 d-flex justify-content-between third-row ">
          <i class="fab devicon-apache-plain"></i>

          <i class="fab devicon-csharp-line-wordmark"></i>
          <i class="fab devicon-cplusplus-line-wordmark"></i>
          <i class="fab devicon-c-line-wordmark"></i>
          <i class="fab fa-linux"></i>
          <i class="fab devicon-github-plain"></i>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.tech {
  background-image: linear-gradient(to bottom right, rgba(0,0,0,0.5), rgba(0,0,0,1)), url(../assets/tech.jpg);
  background-size: cover;
  background-position: center;
  .row {
      height: 100vh;
  }
  .fab {
  color: white;
  font-size: 6rem;
  transition: all .5s;
  
  &:hover {
      color: rgb(16, 104, 204);
      transform: scale(1.2);
  }
}
}



.first-row {
    animation-name: moveFromBottom;
    animation-delay: .5s;
    animation-duration: .5s;
    animation-direction: both;
    animation-timing-function: ease-in;
    animation-fill-mode: forwards;
    opacity: 0;
}

.second-row {
    animation-name: moveFromBottom;
    animation-delay: 1s;
    animation-duration: .5s;
    animation-direction: both;
    animation-timing-function: ease-in;
    animation-fill-mode: forwards;
    opacity: 0;
}
.third-row {
    animation-name: moveFromBottom;
    animation-delay: 1.5s;
    animation-duration: .5s;
    animation-direction: both;
    animation-timing-function: ease-in;
    animation-fill-mode: forwards;
    opacity: 0;
}


    @keyframes moveFromBottom {
        from {
            transform: translateY(2em);
            opacity: 0;
        }
        to {
            transform: translateY(0em);
            opacity: 1;
        }
    }
</style>