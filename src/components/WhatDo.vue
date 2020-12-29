<template>
<div class="whatDo" id="service">
  <div class="container">
    <div class="row">
      <div class='col-12'>
        <div class="do-template">
          <img src="@/assets/aset.png" />
          <div class="do-item">
            <h3>Чем я занимаюсь</h3>
            <div class="frontEnd">
              <i class="fas fa-desktop"></i>
              <p>
                Я Javascript разработчик ,  у меня есть опыт работы с  HTML5 и CSS3 , Bootstrap и jQuery и более продвинутыми фреймворками Javascript, такими как Vue JS и Node JS
              </p>
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
  name:'whatDo'
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Cormorant:wght@600&display=swap');
.whatDo{
  padding-bottom:100px;
}
img{
  width:100%;
}
.do-item{
  width:50%;
  padding-top:50px;
  padding-bottom:50px;
  border:1px solid;
  margin:0 auto;
  position:relative;
  bottom:100px;
  background-color:white;
  text-align:center;
}
.fas{
  font-size:50px;
  padding-top:20px;
  padding-bottom:20px;
}
h3{
  color: #000000;
  font-family: Cormorant;
  font-size: 36px;
  font-weight: 400;
  line-height: 32px;
}
p{
  opacity: 0.9;
  color: #000000;
  font-family: Cormorant;
  font-size: 16px;
  font-weight: 400;
  line-height: 26px;
  letter-spacing: 2px;
  padding-top:1em;
}


@media(max-width:820px){
h3{
  font-size:30px;
}
.fas{
  font-size:45px;
}
.do-item{
  bottom:50px;
}

p{
padding-left:20px;
padding-right:20px;
}

}

@media(max-width:600px){
  .do-item{
    width:60%;
    padding-top:15px;
    padding-bottom:15px;
  }
  .whatDo{
    padding-bottom:60px;
  }

  .do-item{
    width:80%;
    bottom:40px;
  }
}

@media(max-width:450px){
  .fas{
    font-size:40px;
    padding-top:10px;
    padding-bottom:10px;
  }
  h3{
    font-size:28px;
  }
  p{
    padding-top:.5em;
  }

}

@media(max-width:380px){
  h3{
      padding:0px;
      font-size:26px;
  }
  .do-item{
    width:85%;
  }
  p{
    font-size:14px;
    font-weight:800;
  }
  .fas{
    font-size:35px;
  }
}
@media(max-width:330px){
  .do-item{
    width:90%;
    padding-bottom:0px;
  }
  p{
    margin-bottom:3px;
    padding-left:10px;
    padding-right:10px;
  }
  h3{
    font-size:24px;
  }
  .fas{
    padding-top:5px;
  }
}
</style>
