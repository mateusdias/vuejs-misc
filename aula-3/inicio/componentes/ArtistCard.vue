<template>
    <div id="artistcontainer">
        <div id="artistcontent">
            <h1>{{artistName}}</h1>
            <p>{{artistDescription}}</p>
            <p><a href="#">Ouça agora</a></p>
        </div>
    </div>
</template>

<script>
export default {
    props:{
        artistName: String, 
        artistDescription: String
    }
}
</script>

<style scoped>

#artistcontainer{
    margin-top:20px;
    text-align: left;
}

#artistcontent{
    margin: 0 auto;
    padding: 20px;
    width: 70%;
    background-color: rgb(248, 245, 245);
}

#artistcontent h1{
    margin:0;
    padding:0;
    font-size: 22px;
}

#artistcontent p{
    margin-top: 10px;
    margin-bottom:10px;
    padding: 0;
}


</style>