<template>
  <section class="left">
      <ul>
          <li><a class="nav-a" @click="$router.push({name: 'index-right'})">登录</a></li>
          <li><a class="nav-a" @click="$router.push({name: 'index-right2'})">基本信息（公司简介、联系我们）</a></li>
          <li><a class="nav-a">预设模块-组织结构【c模板】</a></li>
          <li><a class="nav-a">预设模块-荣誉【c模板】</a></li>
          <li><a class="nav-a">预设模块-伙伴（合作伙伴）</a></li>
          <li><a class="nav-a">预设模块-公告（主页公告）</a></li>
          <li><a class="nav-a">自定义模块（产品、案例、新闻、下载文件等）</a></li>
          <li><a class="nav-a">文件管理器</a></li>
          <li><a class="nav-a">导航</a></li>
          <li><a class="nav-a">主页</a></li>
          <li><a class="nav-a">海报</a></li>
      </ul>
  </section>
</template>

<script>
export default{
    name:'left',
}
</script>

<style>
.left{
    width: 30%;
    height: 100%;
    float: left;
}
.left ul{
    list-style: none;
    text-align: left;
}
.nav-a{
    padding: 5px 7px;
    display: inline-block;
    width: 100%;
    cursor: pointer;
}
.nav-a:hover{
    text-decoration: underline;
}
</style>
