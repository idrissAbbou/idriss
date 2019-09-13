<template>
  <header class="header d-flex justify-content-center align-items-center">
    <div class="container">
      <div class="row">
        <div class="col-md-6 col-sm-12 d-flex justify-content-center align-items-center">
          <div class="row ">
            <div class="header--title col-12 align-items-center d-flex">
              <h1 class="text-capitalize header--text">
                <span class="hello">Hello I'm</span><span> idriss abbou</span>
              </h1>
            </div>
            <div class="header--icons--col col-12 mt-3">
              <div class="header--icons">
                <a href="https://www.facebook.com/idriss.abbou.77" target="_blank">
                  <i class="icon devicon-facebook-plain"></i>
                </a>
                <a href="https://github.com/idrissAbbou" target="_blank">
                  <i class="icon devicon-github-plain"></i>
                </a>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-sm-12 align-items-center d-flex">
          <div class="card header--card">
            <div class="card-image-top header--image"></div>
            <div class="card-body">
              <h5 class="card-title text-secondary">What I Do</h5>
              <p
                class="card-text text-secondary"
              >A full stack developer, skilled at writing well-designed, testable and efficient code using current best practices in Web development. Fast learner, hard worker and team player.</p>
              <button class="btn btn-outline-secondary btn-block">Download CV</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  components: {}
};
</script>

<style lang="scss">
.header {
  background: linear-gradient(to right bottom, rgba(0, 0, 0, 0.3), black),
    url(../assets/background.png);
  background-position: center;
  height: 100vh;
  color: white;

  &--text {
    animation-name: moveFromBottom;
    animation-delay: 0.5s;
    animation-duration: 1s;
    animation-direction: both;
    animation-timing-function: ease-in;
    animation-fill-mode: forwards;
    opacity: 0;
  }

  &--image {
    height: 250px;
    background-image: linear-gradient(
        to right bottom,
        rgba(0, 0, 0, 0.3),
        rgba(#007fff, 0)
      ),
      url(../assets/gelf.jpg);
    background-size: cover;
  }

  &--icons {
          animation-name: moveFromBottom;
    animation-delay: 0.5s;
    animation-duration: 1s;
    animation-direction: both;
    animation-timing-function: ease-in;
    animation-fill-mode: forwards;
    opacity: 0;
  }
    .hello {
        font-size: 7rem;
        margin-left: -.8rem;
        display: block;
    }
  &--card {
    box-shadow: 1px 1px 2px black;
  }

  .words {
    background-color: rgba(0, 0, 0, 0.5);
  }

  .icon {
      color:white;
      font-size: 3rem;
      padding-right: 1rem;

      &:hover {
          color: gray;
          transform: scale(1.2);
      }
  }


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

  @media (max-width:768px) {
   .header {
     height: 100%;


     &--title, &--icons--col  {
       justify-content: center;
       display: flex;
     }
    &--icons--col {
      margin-bottom: 2rem;
    }
     
     .container {
       margin-top: 4rem;
     }
      h1 {
        text-align: center !important;
        
      }
     .hello {
      font-size: 2.5rem;
      display: inline;
     }

     .icon {
       font-size: 2rem;
     }
   } 
  }

</style>