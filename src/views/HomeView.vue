
<script setup>
import axios from 'axios'
import{ref,reactive,onMounted} from 'vue'

const blogData = ref([])
  async function blog(){
  let url = 'https://basic-blog.teamrabbil.com/api/post-list/2'

 let res = await axios.get(url)
  blogData.value = res
  console.log(res)
}
 blog()


</script>

<template>
  <section class="w-full">
    <div class="w-4/5 mx-auto">
      <div class="w-3/4 mx-auto">
        <img :src="blogData.data[0].img" class="w-full rounded-b">
        <p class="py-2 px-2 border rounded text-base text-blue-950">{{ blogData.data[0].short }} {{ blogData.data[0].short }}</p>
      </div>
      
      
    </div>
  </section>
</template>
