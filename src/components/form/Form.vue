<template>
    <div>
        <form action="">
           <InputTextForm/>
           <InputTextForm/>
           <SubmitForm/>
        </form>
    </div>
</template>


<script>
import InputTextForm from './InputTextForm.vue'
import SubmitForm from './SubmitForm.vue'

export default {
    name: 'Form',
    components: {
        InputTextForm, 
        SubmitForm
    }
}
</script>