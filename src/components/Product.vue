<template>
    <div class="container my-5">
        <b-card title="List Product" sub-title="Product can be add, update and deleted." class="shadow">
            <b-table class="my-3" striped hover responsive  :items="items" :fields="fields"></b-table>
        </b-card>
    </div>
</template>
<script>
export default {
    name: 'Product',
    data() {
        return {
            fields: ['first_name', 'last_name', 'age'],
            items: [
                { isActive: true, age: 40, first_name: 'Dickerson', last_name: 'Macdonald' },
                { isActive: false, age: 21, first_name: 'Larsen', last_name: 'Shaw' },
                { isActive: false, age: 89, first_name: 'Geneva', last_name: 'Wilson' },
                { isActive: true, age: 38, first_name: 'Jami', last_name: 'Carney' }
            ]
        }
    }
}
</script>