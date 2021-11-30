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
  <div v-if="imageSelected">
    <q-btn icon="keyboard_arrow_left" label="이전" color="primary" />
    <q-btn
      icon-right="keyboard_arrow_right"
      label="다음"
      color="primary"
      disable
    />
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
      imageSelected: false,
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
