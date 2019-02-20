<template>
  <div class="about">
    <h1>This is an about page</h1>
    <vue-slider v-if="list.length > 0" :carousel="list"></vue-slider>
  </div>
</template>
<script>
import VueSlider from '_components/vue-slider'
export default {
  name: 'about',
  data() {
    return {
      list: [
        {
          imgUrl: 'http://pic3.iqiyipic.com/common/lego/20190220/b966527c2b3a48abb692547066df949f.jpg'
        },
        {
          imgUrl: 'http://pic3.iqiyipic.com/common/lego/20190219/e680dd0f9e3a4a0c89a56f7daa91d665.jpg'
        },
      ]
    }
  },
  components: {
    VueSlider
  }
}
</script>
