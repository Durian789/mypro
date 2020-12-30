<template>
   <tab-ber>
      <tab-ber-item path="/home" activeColor="red">
        <i slot="item-icon" class="iconfont iconshouye1"></i>
        <i slot="item-icon-active" class="iconfont iconshouye1"></i>
        <div slot="item-text">首页</div>
      </tab-ber-item>
      <tab-ber-item path="/cate" >
        <i slot="item-icon" class="iconfont iconcategory"></i>
        <i slot="item-icon-active" class="iconfont iconleimupinleifenleileibie"></i>
        <div slot="item-text">分类</div>
      </tab-ber-item>
      <tab-ber-item path="/cart" activeColor="blue">
        <i slot="item-icon" class="iconfont iconshop-car-select"></i>
        <i slot="item-icon-active" class="iconfont icongouwuche"></i>
        <div slot="item-text">购物车</div>
      </tab-ber-item>
      <tab-ber-item path="/profile" activeColor="green">
        <i slot="item-icon" class="iconfont iconwode"></i>
        <i slot="item-icon-active" class="iconfont iconwode1"></i>
        <div slot="item-text">我的</div>
      </tab-ber-item>
    </tab-ber>
</template>

<script>
import TabBer from '.././tabber/TabBer'   //导入、注册、使用
import TabBerItem from '.././tabber/TabBerItem'
export default {
  components: {
    TabBer,
    TabBerItem
  }
}
</script>

<style scoped>

</style>