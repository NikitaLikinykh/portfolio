<template>
  <div class="about" id="about">
    <div class="container-fluid">
      <div class="row">
        <div class="col-12">
          <h3>Обо мне</h3>
          <hr />
          <p>
            Привет! меня зовут <b>Никита Ликиных</b>, Front End разработчик, и парень, слегка помешанный на качестве кода. ЕСЛИ У ВАС ЕСТЬ ПРОЕКТ, КОТОРЫЙ ВЫ ХОТИТЕ НАЧАТЬ, ИЛИ ДУМАЕТЕ, ЧТО ВАМ НУЖНА МОЯ ПОМОЩЬ, свяжитесь со мной.
          </p>

          <div class="resume">
            Скачать резюме
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default{
  name:"about"
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Cormorant:wght@600&display=swap');
.about{
  display:block;
  padding-top:120px;
  padding-bottom:100px;
  text-align:center;
  width:70%;
  margin:0 auto;
  text-transform:uppercase;
}
h3{
  color: #000000;
  font-family: Cormorant;
  font-size: 36px;
  font-weight: 400;
  line-height: 32px;
}
p{
  color: #212121;
  font-family: Cormorant;
  font-size: 18px;
  font-weight: 400;
  line-height: 26px;
  padding-top:10px;
  line-height: 30px;
}

.resume{
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
  margin:0 auto;
  margin-top:50px;
}

.resume:hover{
  box-shadow: -1px 10px 18px rgba(0, 0, 0, 0.15);
  background-color: #212121;
  color: #ffffff;
  cursor:pointer;
  transition-duration:0.7s;
}

@media(max-width:820px){
  h3{
    font-size:30px;
  }
  p{
    font-size:16px;
  }
  .about{
    width:80%;
  }
}

@media(max-width:767px){
  .resume{
    width:160px;
    padding-top:5px;
    padding-bottom:5px;
    font-size:14px;
  }
}
@media(max-width:600px){
  h3{
    font-size:28px;
  }
  .resume{
    font-size:13px;
    padding-top:2px;
    padding-bottom:2px;
  }
  .about{
    width:90%;
  }
}

@media(max-width:450px){
  h3{
    font-size:26px;
  }
  p{
    font-size:13px;
  }
  .resume{
    line-height:25px;
  }
}

@media(max-width:380px){
  h3{
    font-size:23px;
  }
}
</style>
