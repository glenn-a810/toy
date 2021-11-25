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
    <p>선택한 이미지 :</p>
  </div>
</template>

<script>
import { defineComponent } from 'vue'
import { date } from 'quasar'

export default defineComponent({
  name: 'PageIndex',
  date: () => [
    {
      id: 1,
      select: false,
      imageName: '',
    },
  ],
})
</script>
