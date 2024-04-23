<template>
    <div class="item-grid">
        <ItemBox v-for="item in items" :key="item._id" :item="item" />
    </div>
</template>

<script>
    import ItemBox from './ItemBox.vue';
    export default{
        name: 'ItemGrid',
        components: {
            ItemBox
        },
        data(){
            return {
                items: []
            };
        },
        mounted(){
            this.fetchItems();
        },
        methods: {
            fetchItems(){
                fetch('https://lennox-beauty-42de7c38e804.herokuapp.com/api')
                    .then(response =>{
                        if(!response.ok){
                            throw new Error(`Error! HTTP Status: ${response.status}`);
                        }
                    return response.json();
                    })
                    .then(data => {
                        this.items = data.map(item => ({
                            ...item,
                            id: item.id
                        }));
                    })
                    .catch(error => {
                        console.error('Unexpected error retrieving data: ', error);
                    });
            }
        }
    };
</script>

<style scoped>
    .item-grid{
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 40px;
        width: 95%;
        max-width: 1200px;
        margin: 0 auto;
        padding-top: 1rem;
    }

    @media(max-width: 768px){
        .item-grid{
            grid-template-colums: 1fr;
        }
    }
</style>