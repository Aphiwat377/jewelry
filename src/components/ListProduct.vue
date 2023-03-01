
<template>
    <!--
-->
<ul>
    <ProductDetall
        v-for="(item, index) in product"
        :id="item.id"
        :key="index"
        :name="item.name"
        :detall="item.detall"
        :type="item.type"
        :price="item.price"
        :picture="item.picture"
        :color="item.color"
        :showDetall="item.showDetall"
        
    />
</ul>
</template>

<script>
import ProductDetall from './ProductDetall.vue';

    export default {
        name: 'ListProduct',
        components:{
            ProductDetall
        },
        data(){
            return {


                product:[
                    {
                        id:1,
                        name:"ÉTINCELLE DE CARTIER",
                        detail:"แหวนเพชร Etincelle de Cartier โรสโกลด์ 750/1000 ประดับเพชรเจียระไนทรงบริลเลียนท์ 46 เม็ด น้ำหนักรวม 0.64 กะรัต จำหน่ายเป็นคู่ ความกว้างของแหวนแต่ละวง 1.52 มม. ความหนา 1.35 มม. (สำหรับขนาด 52)โปรดทราบว่าน้ำหนักกะรัต จำนวนอัญมณี และขนาด อาจแตกต่างกันไปตามขนาดของสินค้าที่คุณสั่งซื้อ โปรดติดต่อเราสำหรับรายละเอียดเพิ่มเติม",
                        type:"แหวน",
                        price:249000,
                        picture:["https://scontent.xx.fbcdn.net/v/t1.15752-9/334014367_517851297063574_2190696322604112583_n.jpg?stp=dst-jpg_p403x403&_nc_cat=110&ccb=1-7&_nc_sid=aee45a&_nc_eui2=AeHC29kb_2lp4oDlMvZzOKICA8hI7NdxurEDyEjs13G6sWh2uYggU4NxpARIHv72fUF6QxQq3HxEmprpfmBDetB8&_nc_ohc=qPat-FxJtboAX_X05lz&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=03_AdRuv7rM0jD8ZrsWszTAElAyWb0VvL09AK43GVODA2u9fw&oe=6423CC23",
                        "https://scontent.xx.fbcdn.net/v/t1.15752-9/334066587_935166614319927_1243900352196170387_n.png?stp=dst-png_s403x403&_nc_cat=105&ccb=1-7&_nc_sid=aee45a&_nc_eui2=AeGAKfCxDvYw8AfWczFAFLj5P9k8qHq0xog_2TyoerTGiOMwAm0ziFiIHhNBZwYq0Qz6zBNSHuU3uLY_tsln3L-Q&_nc_ohc=K8lIbW-kZUcAX__nw7C&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=03_AdRAS7BNGl1OhICiYO51bqToQ1yJjUlDkufPa1P1AAWjCA&oe=6423C933",
                        "https://scontent.xx.fbcdn.net/v/t1.15752-9/327997296_528933942681751_2223905121420604515_n.jpg?stp=dst-jpg_p403x403&_nc_cat=100&ccb=1-7&_nc_sid=aee45a&_nc_eui2=AeEd7bLjB0bBjNa6v6AIi9V6xl6skWWhNxXGXqyRZaE3FYvQLT2nGHSr4mVjco14gjrAUjMTH-MqgHYqzUgF4ZnX&_nc_ohc=p0wozUIRa_AAX9TcccE&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=03_AdTmouNroGmzxcQSSqxLNx5qiT3qnmS8xQbrLPlBb2hQGw&oe=6423E791"],
                        color:"rose gold",
                        showDetall:false,
                    }
                ]


            }
        },
    }
</script>

<style>
    /*@media (min-width: 1024px) {
  .product {

    display: flex;
    align-items: center;
    text-align: center;
    max-height: 500;
    max-width: 600;
    border-style: solid;
    border-color: gold;
  };

  
};
*/

.product {
padding-left: 9px;
display: flex;
align-items: center;
text-align: center;
height: 385px;
width: 225px;
border-style: solid;

border-color: rgb(232, 232, 231);
};

.modal {
  position: fixed;
  z-index: 999;
  top: 20%;
  left: 35%;
  width: 800px;
  margin-left: -150px;
  background-color: white;
  padding: 50px;
    text-align: center;
    border-color: gold;
    border-style: solid;
}
.fancyButton {
    color: #000000;
  background: linear-gradient(315deg, rgb(254, 244, 165) 25%, #ecbd67);
  border: none;
  padding: 5px 10px;
  margin: 5px;
  border-radius: 8px;
  cursor: pointer;
}
.frame{
    display: fiex;
    border-style: solid;
    border-color: gold;
    margin-bottom: 30px;
    
}
.promote{
    height: 200px;
    width: 200px;

}
</style>