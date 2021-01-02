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
  <div class="answer-btn">
      <v-btn
        color="primary"
        x-large
        block
        depressed
      >
        回答する
      </v-btn>
  </div>
      </div>
  </v-container>
</template>

<style>
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
</style>
