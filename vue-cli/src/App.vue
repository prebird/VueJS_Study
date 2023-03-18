<template>
  <div>
    <app-header
     v-bind:propsdata="headerProps"
     v-on:renew="changeHeader">
    </app-header>
  </div>
</template>


<script>
import AppHeader from './components/AppHeader.vue';
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
      headerProps: 'header 입니다.'
    }
  },
  components: {
    'app-header' : AppHeader
  },
  methods: {
    changeHeader: function() {
      this.headerProps = 'hi header 입니다.';
    }
  }
}


</script>

<style>

</style>