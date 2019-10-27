<template>
  <div class="about">
    <h1>This is an about page</h1>
    <button @click="test">test</button>
    <vue-slider v-if="list.length > 0" :carousel="list"></vue-slider>
    <tree></tree>
  </div>
</template>
<script>
import VueSlider from 'components/vue-slider'
import Tree from 'components/tree.vue'
export default {
  name: 'about',
  data() {
    return {
      list: [
        {
          imgUrl: '//pic3.iqiyipic.com/common/lego/20190220/b966527c2b3a48abb692547066df949f.jpg'
        },
        {
          imgUrl: '//pic3.iqiyipic.com/common/lego/20190219/e680dd0f9e3a4a0c89a56f7daa91d665.jpg'
        }
      ]
    }
  },
  methods: {
    test() {
      window.console.log(this)
    }
  },
  components: {
    VueSlider,
    Tree
  }
}
</script>
