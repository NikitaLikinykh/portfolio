<template>
  <div class="works" id="portfolio">
    <h3>Мои работы</h3>
    <hr />
    <div class="container-fluid">
      <div class="row">

        <div class="col-md-6 col-lg-4"  v-for="(work,id) in myworks" :key="id">
          <div class='work-item'>
            <img :src="work.sr" />
          </div>
        </div>


      </div>
    </div>
    <div class="more" @click="addWorks()">
      {{status}}
    </div>
  </div>
</template>

<script>
export default{
  name:"works",
  data(){
    return{
      works:[
        {
          sr:require("@/assets/img_1.png"),
          id:1
        },
        {
          sr:require("@/assets/img_2.png"),
          id:2
        },
        {
          sr:require("@/assets/img_3.png"),
          id:3
        },
        {
          sr:require("@/assets/img_4.png"),
          id:4
        },
        {
          sr:require("@/assets/img_5.png"),
          id:5
        },
        {
          sr:require("@/assets/img_6.png"),
          id:6
        },
        {
          sr:require("@/assets/img_1.png"),
          id:7
        },
        {
          sr:require("@/assets/img_2.png"),
          id:8
        },
        {
          sr:require("@/assets/img_3.png"),
          id:9
        },
        {
          sr:require("@/assets/img_4.png"),
          id:10
        },
        {
          sr:require("@/assets/img_5.png"),
          id:11
        },
        {
          sr:require("@/assets/img_6.png"),
          id:12
        }
      ],
      myworks:[],
      step:6,
      status:"Больше проектов"
    }
  },
  methods:{
    addWorks(){
      this.step+=6;
      this.myworks = this.works.filter(work=>work.id<=this.step)
      this.status = "Больше проектов"
      if(this.step == this.myworks.length){
        this.status = "Скрыть"
      }
      else if(this.step > this.myworks.length){
        this.step = 6
        this.myworks = this.works.filter(work=>work.id<=this.step)
      }
    }
  },
  created(){
      this.myworks = this.works.filter(work=>work.id<=this.step)
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Cormorant:wght@600&display=swap');
  .works{
    padding-bottom:100px;
    text-align:center;
  }
  .work-item{
    padding-top:10px;
    padding-bottom:10px;
  }

  .work-item img{
    width:100%;
  }

h3{
  font-family: Cormorant;
  font-size: 36px;
  font-weight: 400;
  line-height: 32px;
  padding-bottom:80px;
  text-transform:uppercase;
}
hr{
  width:40%;
}
.more{
  width: 174px;
  padding-top:10px;
  padding-bottom:10px;
  border: 1px solid #212121;
  background-color: #ffffff;
  margin-left:10px;

  text-align:center;
  font-family: Cormorant;
  font-size: 15px;
  font-weight: 500;
  line-height: 32px;
  text-transform: uppercase;
  letter-spacing: 1px;
  color: #212121;
  margin:0 auto;
  margin-top:50px;
}

.more:hover{
  box-shadow: -1px 10px 18px rgba(0, 0, 0, 0.15);
  background-color: #212121;
  color: #ffffff;
  cursor:pointer;
  transition-duration:0.7s;
}


@media(max-width:991px){

.work-item img{
  width:90%;
}
.work-item{
  padding-top:15px;
  padding-bottom:15px;
}

}

@media(max-width:820px){
  .work-item img{
    width:90%;
  }
  h3{
    font-size:30px;
  }
}

@media(max-width:767px){
  .work-item img{
    width:75%;
  }
  .more{
    width:160px;
    padding-top:5px;
    padding-bottom:5px;
    font-size:14px;
  }
}
@media(max-width:600px){
  h3{
    font-size:28px;
    padding-bottom:40px;
  }
  .more{
    padding-top:5px;
    padding-bottom:5px;
    font-size:13px;
  }
}

@media(max-width:450px){
  h3{
    font-size:26px;
  }
  .work-item img{
    width:80%;
  }

  .more{
    padding-top:3px;
    padding-bottom:3px;
    line-height:25px;
  }

  .works{
    padding-bottom:50px;
  }

}

@media(max-width:380px){
  h3{
    font-size:22px;
  }
}
</style>
