<template>
  <div class="container-chat-left">
            <aside>
               
              <header>
                <h2>Chats</h2>
                <input type="text" placeholder="Tìm kiếm trên chat...">
              </header>
              <h2 style="margin-left: 20px;">Tin nhắn gần đây</h2>
              <ul>
                <li v-for="chats in chat" :key="chats.id" @click="selectContact()">
                  <img src="chat.User.images" alt="">
                  <span class="status green"></span>
                  <div class="nameUser">
                    <h2>{{chat.User.firstName_lastName}}</h2>
                    <h3>
                     Cho em hỏi shop được ko ạ?
                    </h3>
                   
                  </div>
                  <div class="timechat">3:30 PM</div>
                </li>
              </ul>
            </aside>
    </div>
</template>

<script>
import axios from 'axios';
    export default {
        data(){
          return{
          chat:[]
          }
         
        },
        methods: {
            selectContact() {
                console.log(this.chat)
                axios.get('http://127.0.0.1:8000/api/getallchat').then(response =>(
                        console.log("success"),
                        this.chat=response.data.chat
                    )).catch(error => console.log(error))
                    }
                }
    }
</script>

<style lang="scss" scoped>
.container-chat-left{
    width: 60vh;
    height: 1000px;
    background: #efc7ca;
    margin: 0 20px 30px 50px;
    font-size: 0;
    border-radius: 5px;
    }

aside{
    width: 100%;
    height: 1000px;
    background-color: #f1f6fb;
    display: inline-block;
    font-size: 15px;
    vertical-align: top;
}
aside header{
  padding: 20px 20px;
  line-height: 2.0;
}
aside input{
    width: 85%;
    height: 40px;
    outline: none;
    padding: 0 50px 0 20px;
    background-color: rgb(229, 239, 250);
    border: none;
    border-radius: 3px;
    color: #333;
    // background-image: url(./images/search.png);
    background-repeat: no-repeat;
    background-position: 360px;
    background-size: 25px;
}
::placeholder{
  color:black;
  opacity: 0.5;
  font-family: "Noto Serif", sans-serif;
  font-size: 1.2em;
}
aside ul{
  padding: 10px 0 30px 0;
  margin: 0;
  list-style-type: none;
  height: 690px;
}
aside li{
  display: flex;
  width: 90%;
  background-color: #fff;
  justify-content: space-between;
  border-radius: 10px;
  margin: 20px;
  /* margin-left: 50px; */
  padding: 15px 0 15px 0;
  transition: 1s cubic-bezier(0.65, 0.05, 0.36, 1);
}
aside li:hover{
  background-color:#53b3d0;
  border:none;
  color: #fff;
  border-radius:20px;
  transform: scale(2);
  -moz-transform: scale(1.5,1);
  -webkit-transform: scale(1.5,1);
  -o-transform: scale(1.5,1);
  -ms-transform: scale(1.5,1);
  
}
.nameUser{
  margin-left: -80px;
  font-family: Roboto;
}
.timechat{
  margin-right: 10px;
}
h2,h3{
  margin:0;
}
aside li img{
  border-radius:50%;
  margin-left:20px;
  margin-right:8px;
  width: 50px;
  height: 50px;
}
aside li div{
  display:inline-block;
  vertical-align:top;
  margin-top:12px;
}
aside li h2{
  font-size:14px;
  color:black;
  font-weight:normal;
  margin-bottom:5px;
}
aside li h3{
  font-size:12px;
  color:black;
  font-weight:normal;
}

.status{
  width:8px;
  height:8px;
  border-radius:50%;
  display:inline-block;
  margin-right:7px;
  
}
.green{
  background-color:#58b666;
  margin: 40px 0 0 -125px;
}
.black{
  background-color:#7e818a;
}
.blue{
  background-color:#6fbced;
  margin-right:0;
  margin-left:7px;
}

</style>