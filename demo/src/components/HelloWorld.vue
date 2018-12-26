<template>
  <div class='wraper'>
    <!-- 轮播 -->
    <div class="block">
      <el-carousel height="200px">
        <el-carousel-item v-for="item in swiperData" :key="item">
          <img :src="item.src" alt="">
        </el-carousel-item>
      </el-carousel>
    </div>

  </div>
</template>

<style>
    .wraper {
        width: 100%;
        height: 100%;
    }
    
    .el-carousel__item:nth-child(2n) {
        background-color: #99a9bf;
    }
    
    .el-carousel__item:nth-child(2n+1) {
        background-color: #d3dce6;
    }
    
    .el-carousel__item img {
        width: 100%;
        height: 100%;
    }
</style>

<script>
    export default {
        data() {
            return {
                swiperData: [{
                    "src": "http://pics.sc.chinaz.com/files/pic/webjs1/201511/jiaoben3816.jpg"
                }, {
                    "src": "https://res.yslbeautycn.com/resources/2018/12/19/15452183440963554.jpg"
                }, {
                    "src": "https://res.yslbeautycn.com/resources/2018/11/22/15428756404525620.jpg"
                }, {
                    "src": "https://res.yslbeautycn.com/resources/2018/12/19/15452156657557847.jpg"
                }]
            }
        }
    };
</script>