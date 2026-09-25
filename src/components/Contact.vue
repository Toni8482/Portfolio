<template>
    <div class="section-contact">
        <div class="contact-text">
            <h3>Contacto</h3>
            <p><strong>Email</strong>Toni84822outlook.com</p>
            <p><strong>Github</strong>Toni8482</p>
        </div>
        <div class="contact-form">
            <Form></Form>
        </div>
    </div>
</template>

<script>

import Form from "./Form.vue";
export default {
    name: 'Contact',
    components: {
        Form
    },

    data() {
        return {

        }
    },

    methods: {

    },

    mounted() {

    }
}
</script>

<style scoped>
.section-contact{
    display: flex;
    gap: 30px;
    padding: 150px;
    align-items: start;
    justify-content: center;
}
.contact-text{
    width: 50%;
}

.contact-form{
    width: 50%;
}
</style>