<script setup>
import { reactive, ref } from 'vue';
// const books = ref([
//     {
//         "id": 1,
//         "title": "The Great Gatsby",
//         "author": "F. Scott Fitzgerald",
//         "genre": "Classic Fiction",
//         "publication": "1925"
//     },
//     {
//         "id": 2,
//         "title": "1984",
//         "author": "George Orwell",
//         "genre": "Dystopian Fiction",
//         "publication": "1949"
//     },
//     {
//         "id": 3,
//         "title": "To Kill a Mockingbird",
//         "author": "Harper Lee",
//         "genre": "Classic Fiction",
//         "publication": "1960"
//     },
//     {
//         "id": 4,
//         "title": "The Catcher in the Rye",
//         "author": "J.D. Salinger",
//         "genre": "Coming-of-Age Fiction",
//         "publication": "1951"
//     },
//     {
//         "id": 5,
//         "title": "Pride and Prejudice",
//         "author": "Jane Austen",
//         "genre": "Romantic Fiction",
//         "publication": "1813"
//     }

// ])

</script>

<template>
    <!-- <div>
        <ul v-for="({id, title, author, genre, publication}, index) in books" :key="index">{{ book }}
        
        <li>id:  {{ id }}</li>
        <li>title: {{ title }}</li>
        <li>author: {{ author }}</li>
        <li>genre: {{ genre }}</li>
        <li>publication: {{  publication }}</li>
        
        
        </ul>
    </div> -->

<h1 v-for="(number, index) in 77" :key="index">{{ number }}</h1>

</template>


<style scoped>
h1 {
    color: white;
}
</style>