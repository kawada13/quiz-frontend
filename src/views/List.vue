<template>
  <div class="home">
    <v-container>
      <div class="mt-4">
        <h1 class="text-center">クイズ一覧</h1>
        <h2 class="text-center">カテゴリー名</h2>
      </div>
    <v-row>
      <v-col
          v-for="(item, i) in items"
          :key="i"
          cols="12"
        >
          <v-card
            :color="item.color"
          >
            <div class="d-flex">
              <v-avatar
                class="ma-3"
                size="125"
                tile
              >
                <v-img :src="item.src"></v-img>
              </v-avatar>
              <div>
                <v-card-title
                  class="headline"
                  v-text="item.title"
                ></v-card-title>

                <v-card-subtitle v-text="item.description"></v-card-subtitle>
              </div>
            </div>
          </v-card>
        </v-col>
        <v-col>
          <div class="text-center">
            <v-pagination
              v-model="page"
              :length="6"
            ></v-pagination>
          </div>
        </v-col>
    </v-row>
  </v-container>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

@Component({
  components: {
  },
  data: () => ({
    page: 1,
    items: [
      {
        color: '#FFF',
        src: 'https://cdn.vuetifyjs.com/images/cards/foster.jpg',
        title: 'クイズタイトル',
        description: 'クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容'
      },
      {
        color: '#FFF',
        src: 'https://cdn.vuetifyjs.com/images/cards/halcyon.png',
        title: 'クイズタイトル',
        description: 'クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容'
      },
      {
        color: '#FFF',
        src: 'https://cdn.vuetifyjs.com/images/cards/halcyon.png',
        title: 'クイズタイトル',
        description: 'クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容'
      },
      {
        color: '#FFF',
        src: 'https://cdn.vuetifyjs.com/images/cards/halcyon.png',
        title: 'クイズタイトル',
        description: 'クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容'
      },
      {
        color: '#FFF',
        src: 'https://cdn.vuetifyjs.com/images/cards/halcyon.png',
        title: 'クイズタイトル',
        description: 'クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容'
      },
      {
        color: '#FFF',
        src: 'https://cdn.vuetifyjs.com/images/cards/halcyon.png',
        title: 'クイズタイトル',
        description: 'クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容'
      },
      {
        color: '#FFF',
        src: 'https://cdn.vuetifyjs.com/images/cards/halcyon.png',
        title: 'クイズタイトル',
        description: 'クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容クイズ内容'
      }
    ]
  })
})
export default class Home extends Vue {}
</script>
