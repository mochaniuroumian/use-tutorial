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
          <li><a class="nav-a" @click="$router.push({name: 'index-base'})">基本信息（公司简介、联系我们）</a></li>
          <li><a class="nav-a" @click="$router.push({name: 'index-organization'})">预设模块-组织结构【c模板】</a></li>
          <li><a class="nav-a" @click="$router.push({name: 'index-honor'})">预设模块-荣誉【c模板】</a></li>
          <li><a class="nav-a" @click="$router.push({name: 'index-partner'})">预设模块-伙伴（合作伙伴）</a></li>
          <li><a class="nav-a" @click="$router.push({name: 'index-notice'})">预设模块-公告（主页公告）</a></li>
          <li><a class="nav-a" @click="$router.push({name: 'index-createModule'})">自定义模块</a></li>
          <li><a class="nav-a" @click="$router.push({name: 'index-fileManager'})">文件管理器</a></li>
          <li><a class="nav-a" @click="$router.push({name: 'index-navbar'})">导航</a></li>
          <li><a class="nav-a" @click="$router.push({name: 'index-homepage'})">主页</a></li>
          <li><a class="nav-a" @click="$router.push({name: 'index-poster'})">海报</a></li>
        </ul>
      </section>
      <nuxt-child></nuxt-child>
    </div>
  </div>
</template>

<script>
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
  /* display: -webkit-flex;
  display: flex;
  -webkit-flex-direction: column;
  flex-direction: column; */
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
.left li{
  height: 50px;
}
.left li a{
  line-height: 40px;
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
.main-container{
  width: 69%;
  height: 100%;
  float: left;
}
.page-content{
  padding:20px 10px;
}
.page-content p{
  text-align: left;
  padding:8px 16px;
  text-indent:2em;
}
.page-content .font-pspan{
  padding-left: 4em;
}
.page-content a{
  display: inline;
}
.page-content .font-yellow{
  background-color: yellow;
}
.page-content .font-red{
  color: red;
}
.page-content .content-img img{
  width: 100%;
  border-radius: 8px;
}
.page-content .content-img{
  padding: 10px 40px;
}
</style>
