<template>
  <section>
    <h2>書籍一覧</h2>
    <div class="text-right mb-3">
      <router-link class="btn btn-outline-primary" to="/add">書籍を追加</router-link>
    </div>
    <!--<div class="list-group list-group-flush">-->
        <!--<div class="list-group-item-action" v-for="(book,index) in books" :key="index">{{book.number}} {{book.title}}</div>-->
    <!--</div>-->
    <div class="list-group list-group-flush">
      <router-link :to="`/book/${book.number}`" class="list-group-item-action" v-for="(book,index) in books" :key="index">
        <div class="">{{book.number}} {{book.title}}</div>
      </router-link>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      books: [
        {number: "1", title: "PHPの本"},
        {number: "2", title: "HTMLの本"},
        {number: "3", title: "CSSの本"},
        {number: "4", title: "Javaの本"},
        {number: "5", title: "デザインの本"},
      ]
    }
  }
}
</script>

<style>

</style>
