<template>
  <section class="main-container">
      <div class="page-content">
          <p class="font-red">用户自定义产品、案例、新闻、下载文件等模块</p>
          <p>列表模块（主页显示，适用于多项内容显示，例：产品、案例、新闻等）</p>
          <p>点击左侧导航【设置】-【模块】，列表模块下点击【新增】打开右侧设置界面。</p>
          <p>选择模块类型：<br>
              <span class="font-pspan">文字类适用于多文字的模块<span class="font-yellow">（新闻、资讯、学习资料等）</span></span> <br>
              <span class="font-pspan">图片类适用于图文结合的模块<span class="font-yellow">（应用案例、解决方案等）</span></span> <br>
              <span class="font-pspan">产品类适用于以展示效果为主的模块<span class="font-yellow">（产品展示、服务项目等）</span></span> 
          </p>
          <p>图标svg：svg格式图，建议尺寸400*400，仅用于b模板主页的列表绑定1及c模板手机端主页列表绑定3。</p>
          <p>编辑标识、封面图、简介等信息，点击【确认】完成编辑。右键模块名称可修改、增加子模块、删除模块。</p>
          <p>【选择】图标及封面详见：<a class="nav-a" @click="$router.push({name: 'index-fileManager'})">文件管理器</a></p>
          <div class="content-img">
              <img src="@/static/16-1.jpg">
          </div>
          <br>
          <p>设计模块（主页仅c模板展示一项，适用于图文穿插的自由内容，例：文件下载等）</p>
          <p>点击左侧导航【设置】-【模块】，设计模块下点击【新增】打开右侧设置界面。</p>
          <p>编辑标识、封面图、简介等信息，点击【确认】完成编辑。右键模块名称可修改、增加子模块、删除模块。</p>
          <p>【选择】图标及封面详见：<a class="nav-a" @click="$router.push({name: 'index-fileManager'})">文件管理器</a></p>
          <div class="content-img">
              <img src="@/static/18-1.jpg">
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
