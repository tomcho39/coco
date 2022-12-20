<template>
    <q-card class="town-card">
        <img src="https://cdn.quasar.dev/img/mountains.jpg">
        <q-card-section>
            <div class="text-h6">{{ title }}</div>
            <div class="text-subtitle2">{{subtitle}}</div>
        </q-card-section>
    </q-card>

    <!-- <q-card class="town-card">
      <q-img src="https://cdn.quasar.dev/img/parallax2.jpg">
        <div class="absolute-bottom text-subtitle2 text-center">
          {{title}}
        </div>
      </q-img>
    </q-card> -->
</template>
<script>
import { defineComponent } from 'vue'

/* eslint-disable */
export default defineComponent({
   name: 'ContentCard',

   props: {
    title: { 
        type:String,
        required:true
    },

    subtitle: {
        type:String,
        default:''
    },

    content: {
        type:String,
        default:'1234df'
    }
   }
})
</script>
