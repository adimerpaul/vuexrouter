<template>
  <div>
    <button @click="sumar"><i class="fa fa-plus-circle"></i></button>
    {{num}}
    <button @click="restar"><i class="fa fa-minus-circle"></i></button>
  </div>
</template>
<script>
export default {
  data(){
    return{
      num:1,
    }
  },
  methods:{
    sumar(){
      this.$store.state.numero++;
    },
    restar(){
      this.$store.state.numero--;
    }
  }
}
</script>
