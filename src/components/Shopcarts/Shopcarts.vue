

<template>
    <div>
        <nav-bar title="购物车"></nav-bar>
        <div class="pay-detail">
            <ul>
                <li class="p-list">
                    <mt-switch></mt-switch>
                    <img src="" alt="">
                    <div class="pay-calc">
                        <p>商品标题</p>
                        <div class="calc">
                            <span>￥777</span>
                            <span>-</span>
                            <span>1</span>
                            <span>+</span>
                            <a href="javascript:;">删除</a>
                        </div>
                    </div>
                </li>
            </ul>
        </div>
        <div class="show-price">
            <div class="show-l">
                <p>总计（不含运费）：</p>
                <span>已经选择商品1件，总价￥777元</span>
            </div>
            <div class="show-2">
                <mt-button type="danger" size="large">去结算</mt-button>
            </div>
        </div>
    </div>
</template>

<script>

export default {
  name: '',
  data () {
    return {

    }
  },
  created(){
  }
}

</script>

<style scoped>
      .pay-detail ul li{
          list-style:none;
          margin-bottom:3px;
          border-bottom:1px solid rgba(0,0,0,0.2);
      }
      .pay-detail ul{
         padding-left:5px;
         margin-top:5px;
      }
      .pay-detail ul li img{
         display:inline-block;
         width:80px;
         height:80px;
         vertical-align:middle;
         margin-top:10px;
      }
      .pay-detail ul li:nth-child(1),.pay-detail ul li:nth-child(3){
         display:inline-block;
      }
      .pay-calc p{
         display:inline-block;
         width:250px;
         overflow:hidden;
         color:blue;
         font-size:15px;
         margin-bottom:10px;
      }

       .pay-detail ul li:nth-child(1){
          line-height:80px;
       }
       .calc:nth-child(1){
          color:red;
          font-size:20px;
       }
       .calc span:not(:nth-child(1)){
          dispaly:inline-block;
          width:20px;
          text-align:center;
          border:1px solid rgba(0,0,0,0.3);
       }
       .calc a{
          margin-left:20px;
       }
       .show-1,.show-2{
          display:inline-block;
          margin-left:30px;
       }
       .show-price{
          background:rgba(0,0,0,0.2);
       }
</style>
<!--let goodsList = GoodsTools.getGoodsList();-->
<!--let ids = Object.keys(goodsList).join(',');-->
<!--this.$axios.get('goods/getshopcarlist/'+ids)-->
<!--.then(res=>{-->
<!--this.shopcart= res.data.message;-->
<!--})-->
<!--.catch(err=>console.log('购物车数据异常'));-->

