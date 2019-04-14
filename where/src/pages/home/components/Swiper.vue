<template>
  <div class="wrapper">
    <swiper :options="swiperOption" v-if="showSwiper">
      <swiper-slide v-for="item of list" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl" />
      </swiper-slide>
      <!--滚动                                             -->
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default{
	name: "HomeSwiper",
	data (){
		return{
			swiperOption: {}
		}
	}
}
</script>

<style>
	.swiper-img
	   width: 100%
</style>