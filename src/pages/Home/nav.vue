<template>
<div class="qq">

  <div class="wrap">
    <p class="item">测试</p>
  </div>
</div>
</template>
<script>
export default {
  

}
</script>
<style>
.qq{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%)
}
.wrap{
  min-height: 40px;
  position: relative;
  display: table;
  text-align: center;
  border-radius: 7px;
  background-color: #9EEA6A;
  border: 1px solid #736262;
}
.item{
  display: table-cell;
    vertical-align: middle;
    padding: 0 10px;
}
.wrap:before,.wrap:after{
     content: '';
    display: block;
    width: 0;
    height: 0;
    border: 8px solid transparent;
    position: absolute;
    top: 11px;

    border-right: 8px solid #9EEA6A;
    left: -16px;
}
.wrap::before{
  border-right: 8px solid #736262;
    left: -17px;
    z-index: -1;
}



/* 
.item{
  width: 500px;
}
.item:before{
   content: 'Hello';
   color: red;
}
.item:after{
     content: '';
    display: inline-block;
    width: 0;
    height: 0;
    border: 8px solid transparent;
    border-left: 8px solid #AFABAB;
    position: relative;
    top: 2px;
    left: 10px;
} */
</style>
