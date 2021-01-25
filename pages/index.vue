<template>
  <div class="container">
    <header class="title">
      <h1>
      共享建站使用教程
    </h1>
    </header>
    <div class="main">
      <section class="left">
        <!-- <ul>
          <li><a class="nav-a" @click="$router.push({name: 'index'})">登录</a></li>
          //<li><nuxt-link class="nav-a" to="/right">登录</nuxt-link></li> 
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
        </ul> -->
         <ul>
          <li v-for="(item,index) in lists" :key="index">
            <a @click="preClick(item,index)" class="pre_menu" :class="cur==index?'active':null" :title="item.name">
              <span>{{item.name}}</span>
            </a>
            <ul v-show="cur==index&item.subItems!=null">
              <li v-for="(sub,i) in item.subItems" :key="i">
                <a class="sub_menu" :title="sub.subname" @click="$router.push({name: sub.sunurl})">
                  {{sub.subname}}
                </a>
              </li>
            </ul>
          </li>
        </ul>
      </section>
      <nuxt-child></nuxt-child>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
    cur: null,
      lists: [{
        name: '登录',nameurl:'index',subItems: []
      },{
        name: '基本信息（公司简介、联系我们）',nameurl:'index-base',subItems: []
      },{
        name: '预设模块-组织结构【c模板】',nameurl:'index-organization',subItems: []
      },{
        name: '预设模块-荣誉【c模板】',nameurl:'index-honor',subItems: []
      },{
        name: '预设模块-伙伴（合作伙伴）',nameurl:'index-partner',subItems: []
      },{
        name: '预设模块-公告（主页公告）',nameurl:'index-notice',subItems: []
      },{
        name: '自定义模块',nameurl:'index-createModule',
        subItems: [{
            subname:'建立模块',
            sunurl:'index-createModule'
          },{
            subname:'编辑模块',
            sunurl:'index-editModule'
          }]
      },{
        name: '文件管理器',nameurl:'index-fileManager',subItems: []
      },{
        name: '导航',nameurl:'index-navbar',subItems: []
      },{
        name: '主页',nameurl:'index-homepage',subItems: []
      },{
        name: '海报',nameurl:'index-poster',subItems: []
      }
      ]}
  },
  methods: {
    preClick(item,index) {
      this.cur = this.cur == index ? null : index
      this.$router.push({name: item.nameurl})
     }
  }
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
  height: 18vh;
  width: 100%;
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
  line-height: 18vh;
}
.main{
  width: 100%;
  height: 82vh;
}
.left{
  width: 25%;
  height: 100%;
  float: left;
  border-right: 1px solid #ddd;
  overflow: scroll;
}
.left::-webkit-scrollbar{
  width:4px;
}
.left::-webkit-scrollbar-button{
  display: none;
}
.left ul{
  list-style: none;
  text-align: left;
  padding-left: 0px;
}
/* .left li{
  height: 50px;
} */
.left li a{
  line-height: 30px;
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
  width: 74%;
  height: 100%;
  float: left;
  overflow-y: scroll;
}
.main-container::-webkit-scrollbar{
  width:4px;
}
.main-container::-webkit-scrollbar-button{
  display: none;
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
.pre_menu {
  position: relative;
  padding: 8px 8px 8px 20px;
  font-size: 14px;
  font-weight: 300;
}
.pre_menu::after {
  content: "";
  position: absolute;
  top: 45px;
  left: 0;
  height: .5px;
  width: 100%;
  background-color: rgba(116, 185, 255,0.2)
}
.sub_menu {
  padding:  8px 8px 8px 40px;
  position: relative;
  font-size: 13px;
}
.pre_menu:hover,
.sub_menu:hover {
  cursor: pointer;
}
.sub_menu:hover{
  background: rgb(184, 229, 252, 0.6);
}
.sub_menu::after {
  content: "";
  position: absolute;
  top: 46px;
  left: 0;
  height: 1px;
  width: 100%;
  background-color: #FFFFFF;
}
.left a {
  display: flex;
  justify-content: space-between;
  vertical-align: top;
}
.left a>div {
  transition: .5s;
}
.active{
  background:rgba(116, 185, 255,0.2);
}
</style>
