<template>
  <div class="p-4">
    <b-icon icon="house-door-fill" animation="spin"  ></b-icon> รายการสินค้า <b-icon icon="house-door-fill" animation="spin"  ></b-icon>  
  
      <b-row>

 
  
<b-col>
    <p>Artoria Pendragon <code>24$</code>:</p>
  <b-button class="p-3 mb-2 bg-white text-dark" @click="click11" ><b-img src="https://appmedia.jp/wp-content/uploads/2016/06/c5f3771c96a6c0ed7070e5f63bd0214d.jpg" width="170" ></b-img></b-button>
   <b-col ><b-button size="sm" variant="danger" @click="click11" >ลงรถเข็น <b-badge variant="light">{{click1}}</b-badge></b-button>  <b-button size="sm" variant="danger" @click="click121" >เอาออกรถเข็น </b-button>
   </b-col>
</b-col>
<b-col>
  <p>Artoria Pendragon (Alter) <code>15$</code>:</p>
  <b-button class="p-3 mb-2 bg-white text-dark" @click="click22" ><b-img src="https://www.wicurio.com/grand_order/index.php?plugin=resizeimage&page=%E3%82%A8%E3%82%A4%E3%83%97%E3%83%AA%E3%83%AB%E3%83%95%E3%83%BC%E3%83%AB%EF%BC%88H28%EF%BC%89&w=163&h=280&image=0034128.jpg" width="170"></b-img></b-button>
 <b-col ><b-button size="sm" variant="danger" @click="click22" >ลงรถเข็น <b-badge variant="light">{{click2}}</b-badge></b-button>  <b-button size="sm" variant="danger" @click="click122" >เอาออกรถเข็น </b-button>
   </b-col></b-col>
<b-col>
  <p>Okita Sōji <code>24$</code>:</p>
  <b-button class="p-3 mb-2 bg-white text-dark" @click="click33" ><b-img src="https://i.pinimg.com/236x/34/f5/2f/34f52fdbfa15318e91201feda7a2b6ab.jpg" width="170" ></b-img></b-button>
 <b-col ><b-button size="sm" variant="danger" @click="click33" >ลงรถเข็น <b-badge variant="light">{{click3}}</b-badge></b-button>  <b-button size="sm" variant="danger" @click="click123" >เอาออกรถเข็น </b-button>
   </b-col>
   </b-col>
   </b-row>
   <br>
   <b-row>
  <b-col>
    <p>Astolfo (Saber) <code>24$</code>:</p>
 <b-button class="p-3 mb-2 bg-white text-dark" @click="click44" > <b-img src="https://appmedia.jp/wp-content/uploads/2020/03/b4a5b2165a9271cac91761300c74376e.jpg" width="170"></b-img></b-button>
   <b-col ><b-button size="sm" variant="danger" @click="click44" >ลงรถเข็น <b-badge variant="light">{{click4}}</b-badge></b-button>  <b-button size="sm" variant="danger" @click="click124" >เอาออกรถเข็น </b-button>
   </b-col>
</b-col>
<b-col>
  <p>Astolfo  <code>15$</code>:</p>
 <b-button class="p-3 mb-2 bg-white text-dark" @click="click55" > <b-img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRpCVVIzqyP3u7peTztanjMTuCC-rEF8jhhYA&usqp=CAU" width="170" ></b-img></b-button>
 <b-col ><b-button size="sm" variant="danger" @click="click55" >ลงรถเข็น <b-badge variant="light">{{click5}}</b-badge></b-button> <b-button size="sm" variant="danger" @click="click125" >เอาออกรถเข็น </b-button>
   </b-col></b-col>
<b-col>
  <p>Osakabehime<code>24$</code>:</p>
  <b-button class="p-3 mb-2 bg-white text-dark" @click="click66" ><b-img src="https://www.inside-games.jp/imgs/zoom/793398.jpg"  width="170" ></b-img></b-button>
 <b-col ><b-button size="sm" variant="danger" @click="click66" >ลงรถเข็น <b-badge variant="light">{{click6}}</b-badge></b-button>  <b-button size="sm" variant="danger" @click="click126" >เอาออกรถเข็น </b-button>
   </b-col>
  </b-col>
  </b-row>
  <br>
  <h4><b-icon icon="cart4" animation="spin"  ></b-icon> รายการสินค้าที่สั่งใว้ <b-icon icon="cart4" animation="spin"  ></b-icon></h4>
    <h5>ราคาของทั้งหมด = {{click7}} $</h5>
    <b-col>
    <b-button size="sm" variant="danger" @click="click111" >เอาออกรถเข็นทั้งหมด </b-button> <b-button size="sm" variant="danger" @click="click111" v-on:click="click1111">ตกลง</b-button></b-col>
   </div>
  

</template>

<script>
  export default {
    
    data(){
      return{
        click1:0,
        click2:0,
        click3:0,
        click4:0,
        click5:0,
        click6:0,
        click7:0
      };
    },
    methods:{
     click11 (){
        this.click1++,
        this.click7 +=24;
      },
      click22 (){
        this.click2++,
        this.click7 +=15;
      },
      click33 (){
        this.click3++,
        this.click7 +=24;
      },
      click44 (){
        this.click4++,
        this.click7 +=24;
      },
      click55 (){
        this.click5++,
        this.click7 +=15;
      },
      click66 (){
        this.click6++,
        this.click7 +=24;
      },
      click111(){
        this.click1 =0,
        this.click2 =0,
        this.click3 =0,
        this.click4 =0,
        this.click5 =0,
        this.click6 =0,
        this.click7 =0;
      },
        click121(){
          if(this.click1 >0 ){
         this.click1--,
        this.click7 -=24;}
      },
      click122(){
        if(this.click2 >0 ){
        this.click2--,
        this.click7 -=15;}
      },
      click123(){
        if(this.click3 >0 ){
        this.click3--,
        this.click7 -=24;}
      },
      click124(){
        if(this.click4 >0 ){
        this.click4--,
        this.click7 -=24;}
      },
      click125(){
        if(this.click5 >0 ){
        this.click5--,
        this.click7 -=15;}
      },
      click126(){
        if(this.click6 >0 ){
        this.click6--,
        this.click7 -=24;}
      },
       click1111: function() {
      alert(
        "ขอบคุณที่ใช้บริการ สินค้าที่คุณลูกค้าสั่งนั้นจะถูกจัดส่งให้ในเร็วๆนี้ "
      );
    },
    }
    
  }

</script>
