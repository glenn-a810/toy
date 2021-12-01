<template>
  <q-page class="full-width row justify-start items-center content-start">
    <q-img
      class="col-4 col-md-6"
      src="~assets/img_1.jpg"
      style="max-width: 50%; max-height: 50%; overflow: auto; background: red"
      fit="scale-down"
    />
    <q-img
      class="col-4 col-md-6"
      src="~assets/img_1.jpg"
      style="max-width: 50%; max-height: 50%; overflow: auto; background: blue"
      fit="scale-down"
    />
    <div v-if="imageSelected" class="col-12" style="background: red">
      <q-btn icon="keyboard_arrow_left" label="이전" color="primary" />
      <q-btn
        icon-right="keyboard_arrow_right"
        label="다음"
        color="primary"
        disable
      />
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
