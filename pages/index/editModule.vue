<template>
  <section class="main-container">
      <div class="page-content">
         <p>列表模块</p>
          <p>点击【列表模块】-【模块名称】，点击【新增】进入编辑页面，添加封面、标题（必填）、标签（公告/通知）、图片组（详情页多张图轮播展示）、正文。</p>
          <p>正文插入图片：点击【文件管理器】详见：文件管理器   ，图片居中显示效果最佳。</p>
          <p>文件下载/超链接：点击超链接图标输入地址、显示文字、打开方式等。</p>
          <p><span class="font-yellow">绑定<a class="nav-a" @click="$router.push({name: 'index-navbar'})">导航</a>后可实时查看网站效果</span></p>
          <div class="content-img">
              <img src="@/static/19-1.jpg">
          </div>
          <div class="content-img">
              <img src="@/static/20-1.jpg">
          </div>
          <div class="content-img">
              <img src="@/static/21.png">
          </div>
          <br>
          <p>设计模块</p>
          <p>点击【设计模块】-【模块名称】，点击【新增】进入编辑页面，直接自定义正文内容。</p>
          <p>插入图片：点击【文件管理器】详见：<a class="nav-a" @click="$router.push({name: 'index-fileManager'})">文件管理器</a>，图片居中显示效果最佳。</p>
          <p>文件下载/超链接：点击超链接图标输入地址、显示文字、打开方式等。</p>
          <p><span class="font-yellow">绑定<a class="nav-a" @click="$router.push({name: 'index-navbar'})">导航</a>后可实时查看网站效果</span></p>
          <div class="content-img">
              <img src="@/static/23.jpg">
          </div>
          <div class="content-img">
              <img src="@/static/22.jpg">
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
