<template>
  <div class="hello">
    <div class="col-lg-6">
     <div class="input-group">
       <input v-model="name" type="text" class="form-control" placeholder="ชื่อวิชา">
       <input v-model="phone" type="text" class="form-control" placeholder="หน่วยกิต">
       <input v-model="email" type="text" class="form-control" placeholder="เกรด">
       <span class="input-group-btn">

         <button @click="add(name, phone, email)" class="btn btn-default" type="button">+Add</button>
       </span>
     </div><!-- /input-group -->
   </div><!-- /.col-lg-6 --><br><br><br>
   <center>
  </div><button @click="" class="btn btn-default" type="button" style="background-color: #4CAF50;font-size: 16px;padding: 15px 32px;color: white;">คำนวณ</button></center>
</template>

<script>
export default {
  props: ['add'],
  data () {
    return {
      input: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
</style>
