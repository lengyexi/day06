<template>
  <div>
    <div class="block">
        <el-carousel height="220px">
        <el-carousel-item v-for="item in picList" :key="item">
            <h3 class="small">
                <img :src="item" alt="">
            </h3>
        </el-carousel-item>
        </el-carousel>
    </div>
  </div>
</template>

<script>
export default {
    data () {
        return {
              picList:['https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1567818031&di=be2773d90ea9e3048af1e4e1496d811e&imgtype=jpg&er=1&src=http%3A%2F%2Fpic108.nipic.com%2Ffile%2F20160828%2F21343078_165728899714_2.jpg',
                    'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1567818046&di=2a3ceb54580549ace91d6ba41b69f417&imgtype=jpg&er=1&src=http%3A%2F%2Fpic31.nipic.com%2F20130731%2F13345615_081736258119_2.jpg',
                    'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1567818066&di=bcb0928ea487ac46437e933557bdc9e4&imgtype=jpg&er=1&src=http%3A%2F%2Fpic35.nipic.com%2F20131118%2F3822951_113651482000_2.jpg',
                    'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1567223370766&di=97f2cd58afc04485d906e830e3a26e82&imgtype=0&src=http%3A%2F%2Fpic49.nipic.com%2Ffile%2F20140929%2F4949133_160254012000_2.jpg',
                    ]    
        }
      
    }
}
</script>

<style scoped>
    .el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 150px;
    margin: 0;
  }
  img{
      width: 100%;
      height: 100%;
  }

  .el-carousel__item:nth-child(2n) {
     background-color: #99a9bf;
  }
  
  .el-carousel__item:nth-child(2n+1) {
     background-color: #d3dce6;
  }
</style>