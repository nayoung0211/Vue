<script>
export default{
    props : ["name","age"],
    created(){
        console.log(this.name)
    }
}
</script>

<template>
    <h1>child component</h1>
    <p>Name : {{ name }}</p>
    <p>Age : {{ age }}</p>
    </template>