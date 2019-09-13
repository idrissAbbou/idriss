<template>
  <div class="projects d-flex justify-content-center align-items-center">
    <div class="container">
      <div class="row">
        <div class="col-8">
          <div class="bd-example">
            <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
              <ol class="carousel-indicators">
                <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
                <li data-target="#carouselExampleCaptions" data-slide-to="1"></li>
                <!-- <li data-target="#carouselExampleCaptions" data-slide-to="2"></li> -->
              </ol>
              <div class="carousel-inner">
                <div class="carousel-item active ">
                  <img src="../assets/anime-watch.jpg" class="d-block w-100" alt="..." />
                    <div class="w-100 h-100 bg-success"></div>
                  <div class="carousel-caption d-none d-md-block">
                    <h5 class="">Anime Watch</h5>
                    <p>A website index for gamers and anime lovers</p>
                    <p class="text-left">
                        <spam class="tag html">html</spam>
                        <spam class="tag scss">css</spam>
                    </p>
                    <a href="#" class="btn btn-outline-info btn-block">Visite the website</a>
                  </div>
                </div>
                <div class="carousel-item">
                  <img src="../assets/barcode.jpg" class="d-block w-100" alt="..." />
                  <div class="carousel-caption d-none d-md-block">
                    <h5 class="">c sharp barcode generator</h5>
                    <p>this is a side from a big project where we create a barcode scanner for small busnisses</p>
                    <p class="text-left">
                        <spam class="tag csharp">C#</spam>
                        <spam class="tag dotnet">.net framework</spam>
                    </p>
                    <a href="#" class="btn btn-outline-info btn-block">Download from github</a>
                  </div>
                </div>
              </div>
              <a
                class="carousel-control-prev"
                href="#carouselExampleCaptions"
                role="button"
                data-slide="prev"
              >
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="sr-only">Previous</span>
              </a>
              <a
                class="carousel-control-next"
                href="#carouselExampleCaptions"
                role="button"
                data-slide="next"
              >
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="sr-only">Next</span>
              </a>
            </div>
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
.projects {
  height: 100vh;
  background-image: linear-gradient(
      to bottom right,
      rgba(0, 0, 0, 0.5),
      rgba(0, 0, 0, 1)
    ),
    url(../assets/projects.jpg);
  background-size: cover;


    .tag {
        padding: .2rem .7rem;
        font-weight: bold;
      color: white;
      font-size: .8rem;
    }
  .html {
      background-color: orangered;
  }
  .css {
      background-color: blue;
  }
  .scss {
      background-color: red;
  }
  .csharp, .dotnet{
    background-color: blueviolet;
  }
}
</style>