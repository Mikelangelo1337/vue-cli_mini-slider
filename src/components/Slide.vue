<template lang="">
    <div>
  
        <h2>{{slide.title}}</h2>
        <p>{{slide.text}}</p>
   

    </div>
</template>
<script>
export default {
  props: {
    slide: {
      type: Object,
      default: () => ({})
    }

  },
}
</script>
<style lang="">
    
</style>