<template>
    <section>
        <h2 class="mb-3">{{book.number}} {{book.title}}</h2>
        <div class="mb-5">{{book.body}}</div>
        <h2 class="mb-3">貸出履歴</h2>
        <div class="mb-5">{{history.number}} {{history.name}} {{history.date_from}} {{history.date_to}}</div>
        <router-link class="btn btn-outline-primary" to="/">戻る</router-link>
        <router-link class="btn btn-danger" to="/">この本を削除</router-link>
    </section>
</template>

<script>
    export default {
        data () {
            return {
                book: {
                    number: "1.",
                    title: "本のタイトル",
                    body: "本の詳細"
                },
                history: {
                    number: "1",
                    name: "barbara",
                    date_from: "2019-03-01",
                    date_to: "2019-03-07",
                }
            }
        }
    }
</script>

<style>

</style>