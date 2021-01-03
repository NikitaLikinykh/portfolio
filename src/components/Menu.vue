<template>

    <div class="own-menu">
      <div class="container-fluid menu-wrapper">
        <div class="row">
          <div class="col-6">
            <div class="logo-item">
              <a href="#">likinykh.</a>
            </div>
          </div>

          <div class="col-6">

            <div class="menu-item">
              <ul>
                <li><a href="#home">home</a></li>
                <li><a href="#about">about</a></li>
                <li><a href="#service">service</a></li>
                <li><a href="#portfolio">portfolio</a></li>
                <li><a href="#contact">contact</a></li>
              </ul>
            </div>

            <div class="menu-burger" @click="sm=!sm">
              <i class="fas fa-bars"></i>
            </div>

          </div>
        </div>
      </div>

      <div class="mobile-menu" v-if="sm">
        <div class="mobile-menu-item">
          <ul>
            <li @click="sm=!sm"><a href="#">home</a></li>
            <li @click="sm=!sm"><a href="#about">about</a></li>
            <li @click="sm=!sm"><a href="#service">service</a></li>
            <li @click="sm=!sm"><a href="#portfolio">portfolio</a></li>
            <li @click="sm=!sm"><a href="#contact">contact</a></li>
          </ul>

          <div class="close" @click="sm=!sm">
            <i class="fas fa-times"></i>
          </div>
        </div>
      </div>
    </div>

</template>

<script>
export default{
  name:"own-menu",
  data(){
    return{
      sm:false
    }
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@500&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Cormorant&display=swap');

.own-menu{
  position:absolute;
  top:52px;
  width:100%;
  z-index:2;
}
.logo-item a{
  text-decoration: none;
  color: #212121;
  font-family: Montserrat;
  font-size: 20px;
  font-weight: 700;
  font-style: normal;
  line-height: 32px;
  text-align: left;
  letter-spacing:3px;
  margin-left:70px;
}
.menu-item{
  font-family: Cormorant;
}
.menu-item a {
  text-decoration: none;
  color:#212121;
}
ul{
  display:flex;
  list-style:none;
  text-transform:uppercase;
  justify-content:center;
  padding:0px;
}
li{
  color:#212121;
  font-size:16px;
  font-weight: 400;
  line-height: 32px;
  padding-left:14px;
  padding-right:14px;
}
.menu-burger{
  display:none;
  justify-content:flex-end;
}
.mobile-menu{
  display:none;
  width:100%;
  height:100%;
  background-color:black;
  position:fixed;
  top:0px;
  opacity:.92;
}
.mobile-menu-item{
opacity:1;
color:white;
}
.fa-times{
  color:white;
}


@media(max-width:991px){
  .menu-item{
    display:none;
  }
  .fa-bars{
    padding-right:50px;
    font-size:25px;
  }
  .menu-burger{
    display:flex;
  }
  .mobile-menu{
    display:block;
  }
  ul{
    display:flex;
    flex-direction:column;
    align-items:center;
    margin-top:20%;
  }
  li{
    margin-top:1.2em;
    font-size:25px;
    font-weight:600;
  }
  a{
    text-decoration:none;
    color:white;
  }
  .close{
    position:fixed;
    top:25%;
    left:60%;
    opacity:1;
  }
}

@media(max-width:750px){
  .close{
    top:18%;
    left:65%;
  }
}

@media(max-width:560px){
  .close{
    top:28%;
    left:65%;
  }
  .mobile-menu-item{
  margin-top:200px;
  }
}
@media(max-width:400px){
  .fa-bars{
    padding-right:20px;
  }
}
@media(max-width:450px){
  .logo-item a{
    margin-left:20px;
    font-size:18px;
  }
  .mobile-menu-item li{
  font-size:20px;
  }
}
@media(max-width:290px){
  .fa-bars{
    padding-right:0px;
  }
  .logo-item a{
    margin-left:0px;
  }
}
@media(max-width:250px){
  .mobile-menu-item li{
  font-size:18px;
  }

  .close{
    left:75%;
    top:27%;
    font-size:22px;
  }
}
</style>
