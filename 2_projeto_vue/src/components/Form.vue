<template>
    <form action="">
        <div>
            <InputText/>
        </div>
        <div>
            <InputText/>
        </div>
        <div>
            <p></p>
             <Submit/>
        </div>
    </form>

</template>

<script>
import InputText from './form/InputText.vue'
import Submit from './form/Submit.vue'

    export default {
        name: 'Formu',
        components:{
            InputText,
                Submit
        }
    }
</script>