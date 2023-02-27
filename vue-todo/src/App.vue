<template>
  <div id="app">
      <TodoHeader></TodoHeader> <!-- TodoHeader 의 내용이 그대로 붙는다. -->
      <TodoList></TodoList>
      <TodoInput></TodoInput>
      <TodoFooter></TodoFooter>
  </div>
</template>

<script>
// from 위치의 Vue 파일을 갖고와서, 명명한 import 로 다 받겠다.
import TodoHeader from './components/TodoHeader.vue'
import TodoFooter from './components/TodoFooter.vue'
import TodoList from './components/TodoList.vue'
import TodoInput from './components/TodoInput.vue'

// var my_cmp = {
//   template: '<div> component </div>'
// };

// // script tag loading 해서 하는 방법
// new Vue({
//   el: '',
//   components: { // local component
//     'my_cmp': my_cmp
//   }
// })

export default {
  name:'App',
  components: {
    // 컴포넌트 태그명: 컴포넌트 내용
    'TodoHeader': TodoHeader,
    'TodoFooter': TodoFooter,
    'TodoList': TodoList,
    'TodoInput': TodoInput
  }

}
</script>

<style>

</style>