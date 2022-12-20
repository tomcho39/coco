<template>
  <q-page class="flex flex-center">
    <ContentCard v-for="content in cardList"
    :key="content.title"
    v-bind="content"/>
  </q-page>
</template>

<script>
/* eslint-disable */
import { defineComponent } from 'vue'
import ContentCard from 'components/ContentCard.vue'

const cardList= [
  {
    title:'Test1',
    subtitle:'서브타이틀1'
  },
  {
    title:'Test2',
    subtitle:'서브타이틀2'
  }
]

export default defineComponent({
  name: 'IndexPage',
  components:{
    ContentCard
  },
  setup(){
    return {
      cardList
    }
  }
})
</script>
