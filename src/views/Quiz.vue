<template>
  <v-container>
    <h1 class="text-center">クイズタイトル</h1>
    <div class="question-container">
      <div class="question-number">Q1</div>
      <div class="question-box">日本で一番高い山は？</div>
    <div class="my-5" id="answers">
      <v-row>
          <v-col cols="6">
              <v-btn
              dark
              color="blue"
              x-large
              block
            >
              A: 富士山
            </v-btn>
          </v-col>
          <v-col cols="6">
          <v-btn
          dark
          color="blue"
          x-large
          block
          outlined
        >
          B: 六甲山
        </v-btn>
        </v-col>
      </v-row>
        <v-row>
          <v-col cols="6">
              <v-btn
              dark
              color="blue"
              x-large
              block
              outlined
            >
              C: 阿蘇山
            </v-btn>
          </v-col>
          <v-col cols="6">
          <v-btn
          dark
          color="blue"
          x-large
          block
          outlined
        >
          D: 函館山
        </v-btn>
        </v-col>
      </v-row>
    </div>

<div class="dialog">
  <v-row justify="center">
    <v-dialog
      v-model="dialog"
      persistent
      max-width="600"
    >
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="primary"
          dark
          v-bind="attrs"
          v-on="on"
          x-large
          block
          depressed
        >
          回答する
        </v-btn>
      </template>
      <div class="white py-4">
        <div>
          <div class="text-center blue--text judge-text" v-if="true">
            ○正解！
          </div>
          <div class="text-center red--text judge-text" v-else >
            ×不正解！
          </div>
          <div class="text-center font-weight-bold answear-text">
            正解は「A: 富士山」
          </div>
          <div class="py-3 px-6">
            説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明説明
          </div>
          <div class="mt-3">
            <v-btn
              color="cyan darken-1 white--text"
              dark
              v-on="on"
              depressed
              @click="dialog = false"
              class="text-center qqq mb-4"
            >
              次の問題
            </v-btn>
            <v-btn
              color="primary"
              text
              v-on="on"
              @click="dialog = false"
              class="text-center qqq"
            >
              やめる
            </v-btn>
          </div>
        </div>
      </div>
    </v-dialog>
  </v-row>
</div>
  </div>
  </v-container>
</template>
<script>
export default {
  data () {
    return {
      dialog: false
    }
  }
}
</script>

<style>
.judge-text{
  font-size: 40px;
}
.answear-text{
  font-size: 22px;
}
.question-container{
  margin: 0 30px;
}
.question-number{
  padding-left: 6px;
  font-size: 30px;
}
.question-box{
  padding: 10px;
  border: 1px solid black;
  height: 220px;
  font-size: 30px;
}
.answer-btn{
  margin-top: 50px;
}
.qqq {
  display: block;
  margin: 0 auto;
}
</style>
