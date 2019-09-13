<template>
  <div class="welcome d-flex justify-content-center align-items-center">
    <div class="row h-100">
      <div class="col-md-6 col-sm-12 p-5 d-flex flex-column justify-content-center">
        <h1 class="welcome--title">Hi I hope you will like the tour on my website</h1>
        <p class="welcome--paragraph">this my portfolio a website for you but for me a place where I can show what I can build.
            
        </p>
        <blockquote class="blockquote welcome--blockquote">
          <p
            class="mb-0"
          >Show me the code talking is cheap</p>
          <footer class="blockquote-footer">
            Linus Torvald
            <cite title="Source Title"></cite>
          </footer>
        </blockquote>
      </div>
      <div class="col-md-6 col-sm-12 d-flex align-items-center">
        <img src="../assets/waving-girl.gif" class="w-100" alt />
      </div>

      <button class="btn btn-outline-danger close" @click="closeWelcome">X</button>
    </div>
  </div>
</template>

<script>
export default {
  props: ["welcome"],
  methods: {
    closeWelcome() {
      this.$emit("welcomeColsed", false);
    }
  }
};
</script>

<style lang="scss">
.welcome {
  position: absolute;
  top: 0;
  left: 0;
  height: 100vh;
  width: 100vw;
  background-color: white;
  color: black;

  .close {
    position: absolute;
    top: 2rem;
    right: 2rem;
    padding: 1rem;
    display: block;
  }

}


  @media (max-width: 768px) { 
    .welcome {
      &--title {
        font-size: 1.5rem;
      }
      &--paragraph, &--blockquote {
        font-size: 1rem;
      }

      .close {
        
      }
    }
  }
</style>