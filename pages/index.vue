<template>
  <div class="container">
    <h1 class="title">
      共享建站使用教程
    </h1>
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
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
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
  display: block;
  font-weight: 300;
  font-size: 50px;
  color: #35495e;
  letter-spacing: 1px;
  height: 200px;
  width: 100%;
}

.main{
  width: 100%;
  height: 500px;
}
</style>
