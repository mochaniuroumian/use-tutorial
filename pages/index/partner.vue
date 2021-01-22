<template>
  <section class="main-container">
      <div class="page-content">
          <p>点击左侧导航【伙伴】，点击【新增】进入设置页面，编辑logo、伙伴企业名称、伙伴企业链接、简介等信息，点击【确认】完成编辑。</p>
          <p>点击【重置】清空全部内容，点击【退出新增模式】不保存当前内容。</p>
          <p>【选择】上传伙伴企业logo详见：<a class="nav-a" @click="$router.push({name: 'index-fileManager'})">文件管理器</a></p>
          <p><span class="font-yellow">绑定<a class="nav-a" @click="$router.push({name: 'index-navbar'})">导航</a>后可实时查看网站效果</span></p>
          <div class="content-img">
              <img src="@/static/10.jpg">
          </div>
          <div class="content-img">
              <img src="@/static/11.jpg">
          </div>
          <p class="font-red">注意：<br>
              <span class="font-pspan">1.	logo建议尺寸：200*200</span> <br>
              <span class="font-pspan">2.	伙伴企业链接需完整填写，例：https://www.baidu.com</span> 
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
