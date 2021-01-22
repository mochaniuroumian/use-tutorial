<template>
  <section class="main-container">
      <div class="page-content">
          <p>导航下方轮播图展示设置。点击【设置】-【海报】，鼠标悬浮节点出现功能键，点击【添加】进入编辑页面，输入图片、标题、副标题等信息，点击【保存】完成设置。</p>
          <p>点击【新增】继续设置下一张，点击【删除】删除图片。</p>
           <p>【选择】图片详见：<a class="nav-a" @click="$router.push({name: 'index-fileManager'})">文件管理器</a>，按建议宽度、高度设置图片显示效果最佳。</p>
          <div class="content-img">
              <img src="@/static/30-1.jpg">
          </div>
          <div class="content-img">
              <img src="@/static/31.png">
          </div>
          <p class="font-red">注意：<br>
              <span class="font-pspan">1.	主页建议高度为450，其他节点建议高度为300</span> <br>
              <span class="font-pspan">2.	仅需设置一级导航即可</span> 
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
