<template>
  <div class="skills">
    <h3>Мои Навыки</h3>
    <hr />
    <div class="my-progress">
      <div class="container">
        <div class="row">

          <div class="col-lg-4">
            <p>HTML</p>
            <div class="my-progress-item">
              <div class="progresing html">

              </div>
            </div>
          </div>

          <div class="col-lg-4">
            <p>CSS</p>
            <div class="my-progress-item">
              <div class="progresing csss">

              </div>
            </div>
          </div>

          <div class="col-lg-4">
            <p>Java Script</p>
            <div class="my-progress-item">
              <div class="progresing javascript">

              </div>
            </div>
          </div>

          <div class="col-lg-4">
            <p>JQuery</p>
            <div class="my-progress-item">
              <div class="progresing jquery">

              </div>
            </div>
          </div>

          <div class="col-lg-4">
            <p>Vue JS</p>
            <div class="my-progress-item">
              <div class="progresing vuejs">

              </div>
            </div>
          </div>

          <div class="col-lg-4">
            <p>Node JS</p>
            <div class="my-progress-item">
              <div class="progresing nodejs">

              </div>
            </div>
          </div>


        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default{
    name:"skills"
  }
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Cormorant:wght@600&display=swap');
.skills{
  text-align:center;
  padding-bottom:100px;
}
h3{
  font-family: Cormorant;
  color: #000000;
  font-size: 36px;
  font-weight: 400;
  line-height: 32px;
  text-transform: uppercase;
}
.my-progress-item{
  width:90%;
  border:1px solid;
  height:12px;
  margin-top:20px;
  margin-bottom:20px;
  background-color: #dfdfdf;
}

.my-progress{
  margin-top:50px;
}

.progresing{
  height:100%;
  background-color: #212121;
}
.html{
  width:90%;
}
.csss{
  width:80%;
}
.javascript{
  width:70%;
}
.jquery{
  width:80%;
}
.vuejs{
  width:70%;
}
.nodejs{
  width:60%;
}
p{
  text-align:left;
  color: #000000;
  font-family: Cormorant;
  font-size: 24px;
  font-weight: 400;
  line-height: 32px;
}
hr{
  width:40%;
}


@media(max-width:820px){
  h3{
    font-size:30px;
  }
  p{
    font-size:22px;
  }
}

@media(max-width:600px){
  h3{
    font-size:28px;
  }
  p{
    font-size:20px;
  }
}

@media(max-width:450px){
  h3{
    font-size:26px;
  }
p{
  font-size:18px;
}

.my-progress-item{
  height:10px;
}
}

@media(max-width:380px){
  h3{
    font-size:22px;
  }
  p{
    font-size:16px;
  }
}

</style>
