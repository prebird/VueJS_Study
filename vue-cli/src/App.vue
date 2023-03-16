<template>
  <div> hi hello </div>
</template>


<script>
// 컴포넌트를 공유했을때 데이터 공유가되지 않도록 새객체를 반환하는 형식으로 작성한다
// new Vue({
//   data: function() {
//     return {
//       str: 'hi'
//     }
//   }
// })

export default {
  data:function() {
    return {
      str: 'hi'
    }
  }
}


</script>

<style>

</style>