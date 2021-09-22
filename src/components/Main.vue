<template>
<main>
    <div class="content-main">
        <div class="main-up">
            <button type="button" class="btn btn-outline-primary" @click="addHobby=true" >Add Hobby</button>
            <div  id="main-hidden-div" v-if="addHobby">
                <input v-model="hobby" class="form-control input-hobby" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-sm">
                <button type="button" class="btn btn-outline-success" @click="createHobby"> Send!</button>
            </div>
        </div>
        <div class="main-down">
            <div class="main-sport" v-for="(element, index) in hobbys" :key="index">
                <p class="m-0">{{element}}</p>
            </div>
        </div>
    </div>
</main>
    
</template>

<script>

export default {
    name:'Main',  
     data: function(){
        return {
            addHobby: false,
            hobby:'calcio',
            hobbys: [
                "calcio", "basket", "nuoto"
            ]
        }
    },
    methods:{
        createHobby: function(){
            this.hobbys.push(this.hobby)
            console.log(this.hobbys);
        }
    } 
}
</script>
<style scoped>
.input-hobby{
    display: block;
    width: 30%;
    margin:20px auto;
}
.main-sport{
    width: 40%;
    margin: auto;
    border: 2px solid grey;
    text-align: left;
    padding: 10px;
    margin-top: 20px;

}


</style>
