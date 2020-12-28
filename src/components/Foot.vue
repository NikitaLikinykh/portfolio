<template>
<div class="foot">
  <div class="container-fluid">
    <div class="row">
      <div class="col-12">
        <div class="sotions">

          <div class="circle">
            <a href="#"><i class="fab fa-telegram-plane"></i></a>
          </div>

          <div class="circle">
            <a href="#"><i class="fab fa-instagram"></i></a>
          </div>

          <div class="circle">
            <a href="#"><i class="fab fa-linkedin-in"></i></a>
          </div>

          <div class="circle">
            <a href="#"><i class="fab fa-github"></i></a>
          </div>


        </div>
      </div>

      <div class="col-12">
        <p>
          2020. All Rights Reserved
        </p>
      </div>

    </div>
  </div>
</div>
</template>

<script>
export default{
  name:"foot"
}
</script>

<style scoped>
.foot{
  padding-top:2em;
  padding-bottom:2em;
  background-color:black;
}
.circle{
  width:35px;
  height:35px;
  border-radius:50%;
  border:1px solid;
  color:white;
  margin-left:20px;
  text-align:center;
}
.circle:hover{
  background-color:white;
  transition-duration: .5s;
  cursor:pointer;
}
.circle:hover>a{
  color:blue;
  transition-duration: .5s;
}
.sotions{
  display:flex;
  justify-content: center;
}
.fab{
  font-size:22px;
  padding-top:15%;
}
a{
  color:white;
}
p{
  text-align:center;
  color: #ffffff;
  font-family: Cormorant;
  font-size: 16px;
  font-weight: 400;
  line-height: 32px;
  margin-bottom:0px;
  padding-top:1em;
}
.fas{
  padding-top:7px;
}
.goto:hover>.fas{
  color:black;
}


@media(max-width:450px){
.circle{
  width:28px;
  height:28px;
}
.fab{
  font-size:16px;
}
}
</style>
