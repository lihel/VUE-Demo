<template>
  <div id="firstcomponent">
    <h1>test : {{test}}</h1>
    <h1>url : {{url}}</h1>
    <h1>method:{{method()}}</h1>
    <div id="appp">
        <span v-if="seen">
            隐身
        </span>
    </div>
  </div>


</template>

<script type="text/javascript">
  export default {
    data (){
      return {
        test: "Test",
        url: "www.hahaha.com",
        method: function a() {
          return this.test + "哈哈哈哈"
        },
        seen: false
      }
    }
  }

</script>

