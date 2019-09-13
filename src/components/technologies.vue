<template>
  <div class="tech">
    <div class="container">
      <div class="row tekciy d-flex justify-content-center align-items-center p-4">
        <div class="col-sm-6 col-xs-12 d-flex justify-content-between first-row">
          <i class="fab devicon-html5-plain"></i>
          <i class="fab devicon-css3-plain"></i>
          <i class="fab devicon-bootstrap-plain"></i>
        </div>
        <div class="col-sm-6 col-xs-12 d-flex justify-content-between first-row">
          <i class="fab devicon-sass-original"></i>
          <i class="fab devicon-javascript-plain"></i>
          <i class="fab devicon-vuejs-plain"></i>
        </div>
        <div class="col-sm-6 col-xs-12 d-flex justify-content-between second-row">
          <i class="fab devicon-webpack-plain"></i>
          <i class="fab devicon-babel-plain"></i>
          <i class="fab devicon-php-plain"></i>
        </div>
        <div class="col-sm-6 col-xs-12 d-flex justify-content-between second-row">
          <i class="fab devicon-laravel-plain"></i>
          <i class="fab devicon-wordpress-plain"></i>
          <i class="fab devicon-mysql-plain"></i>
        </div>
        <div class="col-sm-6 col-xs-12 d-flex justify-content-between third-row">
          <i class="fab devicon-apache-plain"></i>
          <i class="fab devicon-csharp-line-wordmark"></i>
          <i class="fab devicon-cplusplus-line-wordmark"></i>
        </div>
        <div class="col-sm-6 col-xs-12 d-flex justify-content-between third-row">
          <i class="fab devicon-c-line-wordmark"></i>
          <i class="fab devicon-linux-plain"></i>
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
  background-image: linear-gradient(
      to bottom right,
      rgba(0, 0, 0, 0.5),
      rgba(0, 0, 0, 1)
    ),
    url(../assets/tech.jpg);
  background-size: cover;
  background-position: center;
  .row {
    height: 100vh;
  }
  .fab {
    color: white;
    font-size: 4rem;
    transition: all 0.5s;

    &:hover {
      color: rgb(16, 104, 204);
      transform: scale(1.2);
    }
  }
}

.first-row {
  animation-name: moveFromBottom;
  animation-delay: 0.5s;
  animation-duration: 0.5s;
  animation-direction: both;
  animation-timing-function: ease-in;
  animation-fill-mode: forwards;
  opacity: 0;
}

.second-row {
  animation-name: moveFromBottom;
  animation-delay: 1s;
  animation-duration: 0.5s;
  animation-direction: both;
  animation-timing-function: ease-in;
  animation-fill-mode: forwards;
  opacity: 0;
}
.third-row {
  animation-name: moveFromBottom;
  animation-delay: 1.5s;
  animation-duration: 0.5s;
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

@media (max-width: 768px) {
  .tech {
    .fab {
      font-size: 2.8rem;
    }
    .tekciy {
      margin-top: 3rem;
    }
  }
}
</style>