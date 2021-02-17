<template>
  <div class="p-4">
    <b-icon icon="house-door-fill" animation="spin"  ></b-icon> รายการสินค้า <b-icon icon="house-door-fill" animation="spin"  ></b-icon>  
  
      <b-row>

 
  
<b-col>
    <p>Artoria Pendragon <code>24$</code>:</p>
  <b-img src="https://static.wikia.nocookie.net/fategrandorder/images/3/3e/AF0002.png/revision/latest/scale-to-width-down/350?cb=20200401130607" ></b-img>
   <b-col ><b-button size="sm" variant="danger" @click="click11" >ลงรถเข็น <b-badge variant="light">{{click1}}</b-badge></b-button>
  
   </b-col>
</b-col>
<b-col>
  <p>Artoria Pendragon (Alter) <code>15$</code>:</p>
  <b-img src="https://static.wikia.nocookie.net/fategrandorder/images/5/57/AF0003.png/revision/latest/scale-to-width-down/350?cb=20200401130442" ></b-img>
 <b-col ><b-button size="sm" variant="danger" @click="click22" >ลงรถเข็น <b-badge variant="light">{{click2}}</b-badge></b-button>
   </b-col></b-col>
<b-col>
  <p>Okita Sōji <code>24$</code>:</p>
  <b-img src="https://static.wikia.nocookie.net/fategrandorder/images/2/28/AF0068.png/revision/latest/scale-to-width-down/350?cb=20180428130759" ></b-img>
 <b-col ><b-button size="sm" variant="danger" @click="click33" >ลงรถเข็น <b-badge variant="light">{{click3}}</b-badge></b-button>
   </b-col>
   </b-col>
   </b-row>
   <b-row>
  <b-col>
    <p>Astolfo (Saber) <code>24$</code>:</p>
  <b-img src="https://static.wikia.nocookie.net/fategrandorder/images/d/dd/AF0270.png/revision/latest/scale-to-width-down/350?cb=20200331215432" ></b-img>
   <b-col ><b-button size="sm" variant="danger" @click="click44" >ลงรถเข็น <b-badge variant="light">{{click4}}</b-badge></b-button>
   </b-col>
</b-col>
<b-col>
  <p>Osakabehime (Archer) <code>15$</code>:</p>
  <b-img src="https://static.wikia.nocookie.net/fategrandorder/images/2/27/AF0262.png/revision/latest/scale-to-width-down/350?cb=20200331213311" ></b-img>
 <b-col ><b-button size="sm" variant="danger" @click="click55" >ลงรถเข็น <b-badge variant="light">{{click5}}</b-badge></b-button>
   </b-col></b-col>
<b-col>
  <p>Sei Shōnagon <code>24$</code>:</p>
  <b-img src="https://static.wikia.nocookie.net/fategrandorder/images/b/b1/AF0276.png/revision/latest/scale-to-width-down/350?cb=20200331220206" ></b-img>
 <b-col ><b-button size="sm" variant="danger" @click="click66" >ลงรถเข็น <b-badge variant="light">{{click6}}</b-badge></b-button>
   </b-col>
  </b-col>
  </b-row>
  <br>
  <h4><b-icon icon="cart4" animation="spin"  ></b-icon> รายการสินค้าที่สั่งใว้ <b-icon icon="cart4" animation="spin"  ></b-icon></h4>
    <h5>ราคาของทั้งหมด = {{click7}}</h5>
    <b-col>
    <b-button size="sm" variant="danger" @click="click111" >เอาออกรถเข็น </b-button> <b-button size="sm" variant="danger" @click="click111" >ตกลง</b-button></b-col>
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
    }
    
  }

</script>
