<script setup>
import axios from "axios";

const response = await axios.get("https://vpic.nhtsa.dot.gov/api/vehicles/getallmanufacturers?format=json");
console.log(response);
</script>


<template>
    <h1>Hello world from breaking bad</h1>
    <div v-for="cool in response">
        <pre>{{cool.Results}}</pre>
    </div>

</template>
<style>
</style>