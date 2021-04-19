<template>
   	<div class="container-chat-center">
                  <div class="msg-header">
                      <div class="msg-header-img">
                          <img src="/images/a2.jpg">
                  </div>
                  <div class="active">
                      <h4> <b>On ho</b></h4>
                      <h6> 1 hour ago...</h6>
                  </div>
              
                  <!-- <img src="./images/close.png" class="close"> -->
          
                  <div class="header-icons">
                      <i class="fa fa-camera"></i>
                      <i class="fa fa-microphone"></i>
                      <i class="fa fa-close"></i>
                  </div>
                  </div>
                  <div class="chat-page">
                  <div class="msg-inbox"> 
                  <div class="chats"> 
                  <div class="msg-page">
                  <div class="received-chats"> 
                  <div class="received-chats-img"> 
                      <img src="images/avatar.jpg">
                  </div>
                  <div class="received-msg"> 
                      <div class="received-msg-inbox"> 
                      <p>Hi!! </p>
                      <span class="time">11:01 PM | October 11</span>
                      </div>
                  </div>
                  </div>
                          
                  <div class="outgoing-chats"> 
                  <div class="outgoing-chats-msg"> 
                  <p>Hi!! </p>
                  <span class="time">11:01 PM | October 11</span>
                  </div>
                  <div class="outgoing-chats-img">
                  <img src="images/a2.jpg">
                  </div>
                  </div>
          
                  <div class="received-chats"> 
                  <div class="received-chats-img"> 
                      <img src="images/avatar.jpg">
                  </div>
                  <div class="received-msg"> 
                      <div class="received-msg-inbox"> 
                      <p>How arre you??? </p>
                      <span class="time">11:01 PM | October 11</span>
                      </div>
                  </div>
                  </div>
                          
                  <div class="outgoing-chats"> 
                  <div class="outgoing-chats-msg"> 
                  <p>I'm find. </p>
                  <span class="time">11:01 PM | October 11</span>
                  </div>
                  <div class="outgoing-chats-img">
                  <img src="images/a2.jpg">
                  </div>
                  </div>
          
                  <div class="received-chats"> 
                  <div class="received-chats-img"> 
                      <img src="images/avatar.jpg">
                  </div>
                  <div class="received-msg"> 
                      <div class="received-msg-inbox"> 
                      <p>Hi!! </p>
                      <span class="time">11:01 PM | October 11</span>
                      </div>
                  </div>
                  </div>
                          
                  <div class="outgoing-chats"> 
                  <div class="outgoing-chats-msg"> 
                  <p>Hi On </p>
                  <span class="time">11:01 PM | October 11</span>
                  </div>
                  <div class="outgoing-chats-img">
                  <img src="images/a2.jpg">
                  </div>
                  </div>
          
              </div>
              </div>
              </div>
              <div class="msg-bottom">
                      <div class="bottom-icons">
                          <i class="fa fa-plus-circle"></i>
                          <!-- <i class="fa fa-camera"></i>
                          <i class="fa fa-microphone"></i>-->
                         
                      </div>
          
                      <div class="input-group">
                          <input class="form-control" type="text" placeholder="write message...">
                          <div class="input-group-append">
                              <span class="input-group-text">
                                 
                                  <i class="fa fa-paper-plane"></i>
                                  <i class="fa fa-smile-o"></i>
                                </span>
                          </div>
                      </div>
              </div>
              </div>
	 </div>
</template>

<script>
    // import MessagesFeed from './MessagesFeed';
    // import MessageComposer from './MessageComposer';
    export default {
        // props: {
        //     contact: {
        //         type: Object,
        //         default: null
        //     },
        //     messages: {
        //         type: Array,
        //         default: []
        //     }
        // },
        // methods: {
        //     sendMessage(text) {
        //         if (!this.contact) {
        //             return;
        //         }
        //         axios.post('/conversation/send', {
        //             contact_id: this.contact.id,
        //             text: text
        //         }).then((response) => {
        //             this.$emit('new', response.data);
        //         })
        //     }
        // },
        // components: {MessagesFeed, MessageComposer}
    }
</script>

<style  scoped>
.container-chat-center {
  width: 60%;
  height: 1000px;
  font-family: sans-serif;
  letter-spacing: 0.5px;
  display: grid;
  border-right: solid rgb(232 228 228);
  border-left: solid rgb(232 228 228);
  border-width: 0.1px;
}
img{
    max-width: 100%;
}
.msg-header{
  width: 95%;
  margin-left: 25px;
  border-radius: 10px;
  height: 90px;
  display: inline-block;
  background-color: #fff;
}
.msg-header-img{
width: 60px;
margin-left: 5%;
margin-top: 12px;
float: left;
}
.msg-header-img img{
border-radius: 100%;
}
.active {
  width: 120px;
  line-height: 1.0em;
  float: left;
  margin-top: 20px;
}
.active h4{
	font-size: 12px;
	color: rgb(56, 55, 55);
	margin-left: 10px;
  /* font-family: cursive; */
}
.active h6{
	font-size: 10px;
	color: #777;
	margin-left: 10px;
}
.header-icons{
  width: 120px;
  float: right;
  margin-top: 25px;
  margin-right: 10px;
}
.header-icons .fa{
	color: #53b3d0;
	cursor: pointer;
	margin: 10px;
  height: 50px;
}
.chat-page{
	/* padding: 0 0 50px 0; */
	width: 100%;
  height: 780px;
}
.msg-inbox{
    border: none;
    overflow: hidden;
    padding-bottom: 0px;
    margin-top: -7px;
    height: 650px;
    border-radius: 0px 0px 0px 0px;
}
.close{
    width: 20px;
    height: 20px;
    margin-left: 535px;
    margin-top: 0px;
}
.chats{
	padding: 30px 15px 0 25px;
}
.msg-page{
	height: 516px;
}
.received-chats{
  height: 15%;
}
.received-chats-img
{
	display: inline-block;
	width: 20px;
	float: left;
}
.received-chats-img img{
	border-radius: 10px;
}
.received-msg{
display: inline-block;
padding:  0 0 0 10px;
vertical-align: top;
width: 92%;
}
.received-msg-inbox{
width: 57%;
}
.received-msg-inbox p{
background: #fff none repeat scroll 0 0;
border-radius: 10px 10px 10px 0px;
color: #646464;
font-size: 14px;
margin: 0;
height: 40px;
padding: 5px 10px 5px 12px ;
width: 100%;
}
.received-msg-inbox .time{
  color: #777;
	display: block;
	font-size: 12px;
	margin: 8px 0 0;
}

/* .time{
	color: #777;
	display: block;
	font-size: 12px;
	margin: 8px 0 0;
} */
.outgoing-chats{
	overflow: hidden;
	margin: 26px 20px;
  height: 15%;
}
.outgoing-chats-img{
	display: inline-block;
	width: 20px;
	float: right;
}
.outgoing-chats-img img{
  border-radius: 10px;
}
.outgoing-chats-msg p{
background:#53b3d0 none repeat scroll 0 0;
color: #fff;
font-size: 14px;
margin: 0;
color: #fff;
padding: 5px 10px 5px 12px;
width: 100%;
height: 40px;
border-radius: 10px 10px 0px 10px;

}
.outgoing-chats-msg{
	float: left;
	width: 46%;
	margin-left: 45%;
}
.outgoing-chats-img{
	display: inline-block;
	width: 20px;
	float:right;
}
.outgoing-chats-msg .time{
  color: #777;
	display: block;
	font-size: 12px;
	margin: 8px 8px 0 0;
}
  .msg-bottom {
    position: relative;
    display: flex;
    height: 90px;
    width: 95%;
    margin-left: 25px;
    border-radius: 10px;
    background-color: #fff;
}

.input-group{
	float: right;
  margin-left: -20px;
  margin-top: 15px;
  outline: none !important;
  border-radius: 20px;
  width: 61% !important;
  background-color: #fff;
}
.form-control{
	border: none !important;
	border-radius: 20px !important;
}
.input-group-text{
	background:transparent !important;
	border: none !important;
}
.input-group .fa{
	color: #53b3d0;
	float: right;
	margin: -10px 15px 10px 0;
}
.input-group .form-control{
  outline: none;
  margin: 22px 0px 0px -90px;
}
.bottom-icons{
	float: left;
	margin-top: 17px;
	width: 30% !important;
	margin-left: 20px;
}
.bottom-icons .fa{
	color: #53b3d0;
	padding: 5px;
  margin-top: 15px;
}
.form-control:focus{
	border-color: none !important;
	box-shadow: none !important;
	border-radius: 20px;
}
#profile-image1{
    max-width: 10%;
    margin: 6px 150px;
}
.container-chat-right{
    margin-left: 10px;
    margin-top: 57px;
}
.col-image{
background-color: #e2c3c3;
width: 50%;
}
.container-name h4{
   margin: auto 150px;
}
.container-name p{
   margin: auto 140px;
}
</style>