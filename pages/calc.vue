<template>
    <div>
        <h1 class="title"> 
            {{mensagem}}
        </h1>

        <b-button type="is-primary" @click="teste()">
            Primary
        </b-button>

        <b-field label="Numero1">
            <b-input v-model="numero1"> Numero1 </b-input>
        </b-field>

        <b-field label="Numero2">
            <b-input v-model="numero2">Numero 2</b-input>
        </b-field>

        <b-button type="is-primary" @click="somar()">
            Somar
        </b-button>

        <b-button type="is-primary" @click="menos()">
            Subtrair
        </b-button>

        <b-button type="is-primary" @click="vezes()">
            Multiplicar
        </b-button>

        <b-button type="is-primary" @click="divisao()">
            Dividir
        </b-button>



        <h3 class="title is-3" >{{resultado}}</h3>

        

    </div>
</template>

<script>
import { SourceMapSource } from 'webpack-sources';

export default {
    data() {
        return { 
            numero1:0,
            numero2: 0,
            resultado: 0
        }
    },
    methods: {
        teste() {
            this.mensagem = "Nova Mensgem"
           
        },

        somar(){ this.resultado =  parseInt(this.numero1) + parseInt(this.numero2)
        },

        menos(){
            this.resultado =  parseInt(this.numero1) - parseInt(this.numero2)
        } ,

        vezes(){
            this.resultado =  parseInt(this.numero1) * parseInt(this.numero2)
        },

        divisao(){
            this.resultado =  parseInt(this.numero1) / parseInt(this.numero2)
        }

    }
}
</script>