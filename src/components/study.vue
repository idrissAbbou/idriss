<template>
  <div class="study d-flex justify-content-center align-items-center">
    <div class="container">
      <div class="row">
        <div class="col-md-6 col-sm-12">
          <div class="border-left border-secondary pl-3">
              <div class="row position-relative">
                  <div class="col-12">
                      <i class="fas fa-bookmark"></i>
                      <h4 class="first-heading">TECHNICIEN SPÉCIALISÉ EN DÉVELOPPEMENT INFORMATIQUE</h4>
                      <p class="first-paragraphe">Institut Spécialisé de Technologie Appliquée</p>
                  </div>
              </div>
              <div class="row">
                  <div class="col-12">
                      <i class="fas fa-bookmark"></i>
                      <h4 class="second-heading">BAC+3 SCIENCE MATHÉMATIQUE A</h4>
                      <p class="second-paragraphe">university ibn zohr agadir</p>
                  </div>
              </div>
              <div class="row">
                  <div class="col-12">
                      <i class="fas fa-bookmark"></i>
                      <h4 class="third-heading">BACCALAURÉAT SCIENCE MATHÉMATIQUE A</h4>
                      <p class="third-paragraphe">école hassan 2 laayoune</p>
                  </div>
              </div>
          </div>
        </div>
        <div class="col-md-6 col-sm-12 justify-ceontent-center align-items-center d-flex">
            <div class="study--cloud d-flex align-items-center justify-content-center">
                <p class="w-75 text-muted">Even so I'm a self thought developer and a lot of what I have learned was through hard work</p>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.study {
  background-image: linear-gradient(to bottom right, rgba(0,0,0,0.5), rgba(0,0,0,1)), url(../assets/study.jpg);
  background-size: cover;
  background-position: center;
  height: 100vh;
  color: white;

  .fas {
      font-size: 2rem;
      color: white;
      position: relative;
      top: 2.5rem;
      right: 1.8rem;
  }

  .first-heading, .first-paragraphe {
    animation-name: moveFromBottom;
    animation-delay: .5s;
    animation-duration: .5s;
    animation-direction: both;
    animation-timing-function: ease-in;
    animation-fill-mode: forwards;
    opacity: 0;
  }


  .second-heading, .second-paragraphe {
    animation-name: moveFromBottom;
    animation-delay: 1s;
    animation-duration: .5s;
    animation-direction: both;
    animation-timing-function: ease-in;
    animation-fill-mode: forwards;
    opacity: 0;
  }


  .third-heading, .third-paragraphe {
    animation-name: moveFromBottom;
    animation-delay: 1.5s;
    animation-duration: .5s;
    animation-direction: both;
    animation-timing-function: ease-in;
    animation-fill-mode: forwards;
    opacity: 0;
  }

  &--cloud {
      height: 100%;

      p{
          margin-top: 5rem;
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
</style>