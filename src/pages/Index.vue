<template>
  <q-page class="flex flex-center">
    <q-img
      src="~assets/img_1.jpg"
      style="max-width: 500px; max-height: 500px"
      fit="scale-down"
    />
    <q-img
      src="~assets/img_1.jpg"
      style="max-width: 500px; max-height: 500px"
      fit="scale-down"
    />
  </q-page>
  <div>
    <!--    <p>선택한 이미지 : {{ imageName }}</p>-->
    <input v-model="imageText" />
  </div>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'PageIndex',
  data: () => {
    return {
      imageText: '',
    }
  },
  // setup() {
  //   const imageName = 'img_1.jpg'
  //   return {
  //     imageName,
  //   }
  // },
})
</script>
