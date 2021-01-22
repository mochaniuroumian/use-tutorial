<template>
  <section class="main-container">
      <div class="page-content">
          <p>点击左侧导航【荣誉】，点击【新增】进入设置页面，编辑证书、名称、起止时间（留空不显示）、简介等信息，点击【确认】完成编辑。</p>
          <p>点击【重置】清空全部内容，点击【退出新增模式】不保存当前内容。</p>
          <p>【选择】上传荣誉证书详见：<a class="nav-a" @click="$router.push({name: 'index-fileManager'})">文件管理器</a></p>
          <p><span class="font-yellow">绑定<a class="nav-a" @click="$router.push({name: 'index-navbar'})">导航</a>后可实时查看网站效果</span></p>
          <div class="content-img">
              <img src="@/static/7-1.jpg">
          </div>
          <div class="content-img">
              <img src="@/static/8.jpg">
          </div>
      </div>
  </section>
</template>

<script>
export default{
}
</script>

<style>
</style>
