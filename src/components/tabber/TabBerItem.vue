<template>
  <div class="tab-ber-item" @click="itemClick">
    <div v-if="isActive" ><slot name="item-icon"></slot></div>
    <div v-else><slot name="item-icon-active"></slot></div>
   <div :style="activeStyle" >
      <slot  name="item-text"></slot>
   </div>
    
  </div>

</template>

<script>
export default {
  props: {
    path: String,
    activeColor:{
      type: String,
      default: 'red'
    }
  },
  data() {
    return {
      // isActive: true,
    }
  },
  methods: {
    itemClick() {
      // console.log('itemClick');
      this.$router.replace(this.path)
    }
  },
  computed: {
    isActive() {
      return this.$route.path.indexOf(this.path) !== -1   //找到了
    },
    activeStyle() {
      return this.isActive ? {color: this.activeColor} : {}
    }
  }
};
</script>

<style scoped>
@import "../../assets/img/tabber/tabber图标/iconfont.css";
.tab-ber-item {
  flex: 1;
  text-align: center;
  height: 49px;
  /* line-height: 49px; */
  font-size: 14px;
}

.tab-ber-item .iconfont {
  font-size: 24px;
  margin-top: 3px;
  margin-bottom: 2px;
}

/* .active {
  color: red;
} */
</style>