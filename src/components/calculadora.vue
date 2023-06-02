<template>
  <h3>num 1  </h3>
  <input type="text" v-model="num1"> *
  <input type="text" v-model="num2">
  <button @click="sumar"> resultado</button>
  <p>{{ resul }}</p>
</template>

<script>
// console.log();
export default {
    data(){
        return{
            num1:'',
            num2:'',
            resul:0
        }
    },
    methods:{
        sumar(){
            const numero1=parseFloat(this.num1);
            const numero2=parseFloat(this.num2);
            // const resultado=
            
            if (!isNaN(numero1) &&  !isNaN(numero2)) {
                this.resul=numero1 * numero2;
            } else {
                console.log("vacio");
                
            }
            // this.resul=this.num1 + this.num2;
        }
    }
}


</script>