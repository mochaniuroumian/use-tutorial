<template>
  <div class="container">
    <header class="title">
      <h1>
      共享建站使用教程
    </h1>
    </header>
    <div class="main">
      <section class="left">
        <ul>
          <li><a class="nav-a" @click="$router.push({name: 'index'})">登录</a></li>
          <!-- <li><nuxt-link class="nav-a" to="/right">登录</nuxt-link></li> -->
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
      <nuxt-child></nuxt-child>
    </div>
  </div>
</template>

<script>
// import left from '../components/left'
// import right from '../components/right'
export default {
  components: {  }
  }
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  width: 100%;
  justify-content: center;
  align-items: center;
  text-align: center;
  display: -webkit-flex;
  display: flex;
  -webkit-flex-direction: column;
  flex-direction: column;
}

.title {
  display: block;
  height: 170px;
  width: 100%;
  padding:20px 10px;
}
.title h1{
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-weight: 300;
  font-size: 50px;
  color: #35495e;
  letter-spacing: 1px;
  line-height: 100px;
}
.main{
  width: 100%;
  height: 500px;
}
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
    text-decoration: none;
    color: #35495e;
}
.nav-a:hover{
    text-decoration: underline;
}
</style>
