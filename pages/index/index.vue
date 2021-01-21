<template>
  <section class="right">
      222<li><a class="nav-a" @click="$router.push({name: 'index-right2'})">基本信息（公司简介、联系我们）</a></li>
  </section>
</template>

<script>
export default{
    name:'Right',
}
</script>

<style>
.right{
    width: 69%;
    height: 100%;
    float: left;
}
</style>
