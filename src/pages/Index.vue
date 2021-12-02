<template>
  <q-page class="full-width row items-center content-start q-pa-xs">
    <q-img
      class="col-6"
      src="~assets/img_1.jpg"
      style="max-width: 100%; max-height: 100%; overflow: auto; background: red"
      fit="scale-down"
    />
    <q-img
      class="col-6"
      src="~assets/img_1.jpg"
      style="
        max-width: 100%;
        max-height: 100%;
        overflow: auto;
        background: blue;
      "
      fit="scale-down"
    />
    <div v-if="imageSelected" class="q-pa-md q-gutter-x-md">
      <q-btn icon="keyboard_arrow_left" label="이전" color="primary" />
      <q-btn icon-right="keyboard_arrow_right" label="다음" color="primary" />
      <p>선택한 이미지 : {{ imageSelected }}</p>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'PageIndex',
  data: () => {
    return {
      imageSelected: true,
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
