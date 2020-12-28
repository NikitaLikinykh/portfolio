<template>
  <div class="explore" id="home">
    <div class="container-fluid">
      <div class="row">

        <div class="col-md-6">
          <div class="hire">
            <div class="description">
              <h4>Никита Ликиных</h4>
              <p>Front-End Разработчик</p>

              <div class="explore-buttons">

                <div class="hire-me">
                  Нанять меня
                </div>

                <div class="explore-more">
                  Узнать Больше
                </div>
              </div>

            </div>

            <div class="cub">

            </div>

          </div>
        </div>

        <div class="col-md-6">
          <div class="profile">
            <img src="@/assets/person.png" />
          </div>
        </div>

      </div>
    </div>
  </div>
</template>

<script>
  export default{
    name:"explore",
    components:{
    }
  }
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Cormorant:wght@600&display=swap');
.hire{
  height:700px;
  max-height:700px;
}

.profile{
  background-color: #e1e1e1;
  height:700px;
  max-height:700px;
}
.description{
  height:100%;
  display:flex;
  flex-direction:column;
  align-items:center;
  justify-content: center;
}
h4{
  color: #212121;
  font-family: Cormorant;
  font-size: 40px;
  font-weight: 700;
  line-height: 50px;
  text-transform: uppercase;
  letter-spacing:3px;
}
p{
  opacity: 0.9;
  color: #212121;
  font-family: Cormorant;
  font-size: 22px;
  font-weight: 400;
  line-height: 32px;
  letter-spacing:2px;
}
.explore-buttons{
  display:flex;
  margin-top:2em;
}
.hire-me{
  width:144px;
  padding-top:10px;
  padding-bottom:10px;
  text-align:center;
  font-family: Cormorant;
  font-size: 16px;
  font-weight: 500;
  line-height: 32px;
  text-transform: uppercase;
  letter-spacing: 1px;
  border: 1px solid #212121;
  color: #212121;
}
.hire-me:hover{
  box-shadow: -1px 10px 18px rgba(0, 0, 0, 0.15);
  background-color: #212121;
  color: #ffffff;
  cursor:pointer;
  transition-duration:0.7s;
}
.explore-more{
  width: 174px;
  padding-top:10px;
  padding-bottom:10px;
  border: 1px solid #212121;
  background-color: #ffffff;
  margin-left:10px;

  text-align:center;
  font-family: Cormorant;
  font-size: 16px;
  font-weight: 500;
  line-height: 32px;
  text-transform: uppercase;
  letter-spacing: 1px;
  color: #212121;
}

.explore-more:hover{
  box-shadow: -1px 10px 18px rgba(0, 0, 0, 0.15);
  background-color: #212121;
  color: #ffffff;
  cursor:pointer;
  transition-duration:0.7s;
}

.cub{
  width:450px;
  height:490px;
  border: 17px solid #212121;
  opacity: 0.1;
  position:absolute;
  top:20%;
  right:45%;
  z-index:-1;
}
.profile{
  text-align:center;
}
img{
  position:absolute;
  width:65%;
  bottom:0px;
  left:20%;
  z-index:1;
}



@media(max-width:991px){
  .hire{
    height:550px;
    max-height:550px;
  }

  .profile{
    height:550px;
    max-height:550px;
  }

  img{
    width:70%;
    max-width:70%;
  }
  .cub{
    width:500px;
    height:450px;
  }
}



@media(max-width:924px){
  h4{
    font-size:30px;
  }
  .hire-me{
    font-size:15px;
    padding-left:2px;
    padding-right:2px;
  }
  .explore-more{
    padding-top:3px;
    padding-bottom:3px;
    font-size:15px;
    padding-left:2px;
    padding-right:2px;
  }
  .explore-buttons{
    margin-top:1em;
  }
}

@media(max-width:767px){
  img{
    width:50%;
    left:30%;
  }

  .profile{
    margin-top:2em;
  }

  .hire-me{
    font-size:13px;
    padding:0px;
  }
    .explore-more{
      font-size:13px;
      padding:0px;
    }
}

@media(max-width:600px){
  .cub{
    width:500px;
    height:400px;
  }
}

@media(max-width:450px){
  .cub{
    height:350px;
  }
  h4{
    font-size:26px;
  }

  p{
    font-size:20px;
  }
  .profile{
    margin-top:0px;
    height:400px;
    max-height:400px;
  }
}
@media(max-width:380px){
  .profile{
    height:300px;
    max-height:300px;
  }
}

@media(max-width:360px){
  .explore-buttons{
    flex-direction:column;
  }
  .explore-more{
    margin-left:0px;
    width:144px;
    margin-top:1em;
  }
}

@media(max-width:335px){
  h4{
    font-size:22px;
  }
}

@media(max-width:305px){
  .profile{
    height:250px;
    max-height:250px;
  }
  img{
    width:55%;
  }
  p{
    font-size:16px;
  }
}
</style>
