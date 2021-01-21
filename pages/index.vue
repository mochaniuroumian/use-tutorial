<template>
  <div class="container">
    <header class="title">
      <h1>
      共享建站使用教程
    </h1>
    </header>
    <div class="main">
      <left></left>
      <right></right>
    </div>
  </div>
</template>

<script>
import left from '../components/left'
import right from '../components/right'
export default {
  components: { left,right }
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
}

.title {
  display: block;
  height: 200px;
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
</style>
