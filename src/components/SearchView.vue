<template>
    <div class="main">
        <input type="text" placeholder="Type in your city...">
        <button>Search</button>

    </div>
</template>

<script>

    export default {
        name: "SearchWindow",
        props: {
            msg: String
        }
    }

</script>


<style scoped>
    .main {
        background-color: blueviolet;
        height: calc(100vh - 66px);
        border-top: 1px solid azure;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .main input {
        width: 500px;
        height: 40px;
        border: 1px solid lightgrey;
        border-radius: 16px;
    }

    .main button {
        width: 150px;
        height: 50px;
        border: none;
        border-radius: 16px;
    }

    
</style>
