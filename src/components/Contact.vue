<template>
  <div class="contact" id="contact">
    <h3>Контакт</h3>
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <form>
            <input type="text" placeholder="Name" class="data" />
            <input type="text" placeholder="E-mail" class="email" />
            <input type="text" placeholder="Message" class="message"/>
            <button type="submit">Нанять меня <i class="far fa-paper-plane"></i></button>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default{
  name:"contact"
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Cormorant:wght@600&display=swap');
h3{
  font-size: 36px;
  font-weight: 400;
  line-height: 32px;
  font-family: Cormorant;
  text-align:center;
  padding-bottom:100px;
}
  .contact{
    padding-bottom:100px;
  }
  .message{
    width:100%;
    margin-top:150px;
  }
  .data{
    width:48%;
  }
  .email{
    width:48%;
    margin-left:4%;
  }
  input{
    border:none;
    border-bottom:1px solid;
    outline: none;
  }
  placeholder{
    font-size: 16px;
    font-family: Cormorant;
    font-weight: 400;
    line-height: 32px;
    text-transform:uppercase;
  }

  button{
    display:block;
    margin:0 auto;
    margin-top:100px;
    width:15%;
    height:40px;
    border: 1px solid #212121;
    box-shadow: -1px 14px 24px rgba(0, 0, 0, 0.18);
    background-color: #ffffff;
    opacity: 0.67;
    color: #212121;
    font-family: Cormorant;
    padding:0px;
  }
  button:hover{
     background-color:black;
     opacity:1;
     color:white;
     transition-duration:.5s;
  }
  .far{
    padding-left:5px;
  }

  @media(max-width:991px){
    button{
      width:20%;
    }
  }


  @media(max-width:820px){
    h3{
      font-size:30px;
    }

    .message{
      width:90%;
      margin-left:10%;
    }
    .data{
      width:40%;
      margin-left:10%;
    }
    .email{
      width:40%;
      margin-left:10%;
    }

  }

  @media(max-width:767px){
    h3{
      padding-bottom:50px;
    }
    .message{
      margin-top:100px;
    }
    button{
      margin-top:80px;
      width:25%;
    }
  }

    @media(max-width:600px){
      h3{
        font-size:28px;
      }
    }

    @media(max-width:450px){
      h3{
        font-size:26px;
      }
      button{
        margin-top:60px;
        width:35%;
        line-height:20px;
      }
    }

    @media(max-width:360px){
      button{
        width:40%;
      }
    }
</style>
