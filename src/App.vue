// 컴포넌트 Refs
<template>
  <!-- <h1 id="hello">
    Hello World!
  </h1> -->
  <!-- <h1 ref="hello">
    Hello World!
  </h1> -->
  <Hello ref="hello" />
</template>

<script>
import Hello from '~/components/Hello'

export default {
  components: {
    Hello
  },
  created() {
    console.log(this.$refs.hello)
  },
  mounted() {
    // const h1El = document.querySelector('#hello')
    // console.log(h1El.textContent)
    console.log(this.$refs.hello.$refs.good)
  }
}
</script>