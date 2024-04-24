<template>
    

    <div  :class="book.availability ? 'green': 'red' ">

                        <h2>{{book.locationname}}</h2>
                        <h4>Best Place in this Location : {{book.location}}</h4>
                        <h4>Hotel Dates(DD.MM) : {{book.hoteldates}}</h4>
                        <h4>Best Time to Visit : {{book.besttimetovisit}}</h4>
                        <h4>Price of the Hotel(dollars) : {{book.price}}</h4>
                        <img :src="book.photo" alt="Hotel Photo" style="max-width: 100%;" />
 
                        
    </div>
</template>

<script>

export default{
    name: 'SingleBook',
    props:{
        book: Array
    }
}
</script>

<style scoped>

.green{
    background-color: green;
}

h4{
    margin: 2px;
}

div{
    background-color: #ffb89e;
    color: black;
    padding: 1em;
    text-align: center;
    width: 80%;
    margin: auto;
    

}

.red{
background-color: orangered !important;

}


</style>