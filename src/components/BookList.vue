<template>
    <div>
        <h1>{{title}}</h1>
        <ul>
            <li v-for="book in books">{{book.title}}:{{book.author}}</li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: 'BookList',
        data() {
            return {
                title: 'All Books',
                books: [
                    {title: 'Self-Reliance', author: 'RalphWaldo Emerson'},
                    {title: 'American news', author: 'Neil Gaiman'},
                    {title: 'Amusing Ourselves', author: 'Postman'}

                ]
            }
        }
    }
</script>

<style>
    h1, h2 {
        font-weight: normal
    }
    ul {
        list-style-type: none;
        padding: 0;
    }
    li {
        display: block;
        margin: 0 10px;
    }
</style>