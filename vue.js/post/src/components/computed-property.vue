<template>
    <h1>Computed property</h1>
    <!-- <p>Has published books:</p>
    <span>{{ publishedBooksMessage }}</span> -->
    <span>{{ getTotal }}</span>
</template>

<script>
    export default{
        name: "computed-property-component",
        data() {
            return {
                // author : {
                //     name: 'John Doe',
                //     books: [
                //         'Vue 2 - Advanced Guide',
                //         'Vue 3 - Basic Guide',
                //         'Vue 4 - The Mystery'
                //     ],
                // },
                cashinhand: 200,
                balance: 50,
                discount: 160,
            };
        },
        computed: {
        //     // a computed getter
        //     publishedBooksMessage() {
        //         // 'this' points to the component instance
        //         return this.author.books.length > 0 ? "Yes" : "No";
        //     },
            getTotal(){
                return this.cashinhand * this.balance - this.discount;
            },
        }
    }
</script>
