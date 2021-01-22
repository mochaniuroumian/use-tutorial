<template>
  <section class="main-container">
      <div class="page-content">
          <p>点击左侧导航【组织结构】进入设置页面，右键选择【编辑】或【扩展】结构内容，同级节点可上下拖动调整显示顺序。</p>
          <p><span class="font-yellow">绑定<a class="nav-a" @click="$router.push({name: 'index-navbar'})">导航</a>后可实时查看网站效果</span></p>
          <div class="content-img">
              <img src="@/static/4.jpg">
          </div>
          <div class="content-img">
              <img src="@/static/5.jpg">
          </div>
          <p class="font-red">注意：<br>
              <span class="font-pspan">1.	根节点不可删除</span> <br>
              <span class="font-pspan">2.	同级节点名称不能重复</span> <br>
              <span class="font-pspan">3.	删除节点时其子内容会全部删除</span> <br>
              <span class="font-pspan">4.	结构图最多5列显示效果最佳</span> 
          </p>
      </div>
  </section>
</template>

<script>
export default{
}
</script>

<style>
</style>
