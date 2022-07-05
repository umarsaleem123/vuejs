<!-- <template>
    <div>
        <h1>{{message}}</h1>
        <textarea type="text" v-model="message" />

    </div>
</template>
<script>


export default {
   // name:'homebind',
    data(){
        return{
            message:'hi'
        }
    }
        
    
}
</script>
<style>
h1{
    white-space: pre-line;
}
</style> -->




<!-- <template>
<div>
<h2 v-for="(name,index) in names" :key="name">{{index}}{{name}}</h2> 
<h3 v-for="(name,i) in fullNames" :key="name.first">{{i}} {{name.first}} {{name.last}}</h3> 


</div>
</template>
<script>
export default{
  name:'databind',
  data(){
    return{
      names:['umair','ahmed','saad'],
      fullNames:[
            {first:'umair', last:'qureshi'},
            {first:'ahmed', last:'saim'},
            {first:'saad', last:'rehman'}
      ],
    }
  },
}
</script> -->

<template>
<div>
    <button v-on:click="hello('data')">call hello function</button>
</div>

</template>
<script>
export default {
    name:'databind',
    props:{
        data:String,
        msg:String
        
    },methods: {
        hello(item){
            console.log(item);
        }
    }
 
}
</script>


