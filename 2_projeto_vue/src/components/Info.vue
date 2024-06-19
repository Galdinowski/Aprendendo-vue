<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades</p>
        <p>Utilizo as seguintes tecnologias:</p>
            <ul>
                <li>JavaScript</li>
                <li>PHP</li>
                <li>Python</li>
            </ul>
            <div>
                <button @click="ShowEmail">{{ textoBotao }}</button>
            </div>
            <p v-show="mostrar_email">Mande uma msg para: {{ email }} </p>
            <p>Para acessar meu portfolio basta <a v-bind:href="meu_link" target="blank"> clicar aqui</a></p>
            <Pictures/>
    </div>

</template>

<script>
    import Pictures from "./Picture.vue"
    export default{
        name: 'Info',
        components:{
            Pictures
        },
        data()
        {
            return{
                esta_trabalhando: true,
                mostrar_email:false,
                email: "Testando@gmail.com",
                meu_link: 'https://www.globo.com/',
                textoBotao: "Mostrar e-mail"

            }
        },
        methods:{
            ShowEmail(){
                this.mostrar_email = !this.mostrar_email
                if(!this.mostrar_email)
                 {
                       this.textoBotao = "Mostrar E-mail"
                       
                       
                    }else{
                        this.textoBotao = "Esconder E-mail"
                    }
            }
        }

}
</script>