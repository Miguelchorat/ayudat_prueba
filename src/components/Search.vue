<template>
    <form class="search">
        <input class="search__input" type="email" ref="emailInput" :placeholder="placeholderText" aria-label="email" v-model="search">
        <a class="search__button" href="#" @click="handleSubmit">Suscribe</a>
    </form>
</template>

<script>
export default {
    name: 'SearchComponent',
    data() {
        return {
            search: '',
            isEmailValid: true,
            placeholderText: 'Your email'
        }
    },
    methods: {
        handleSubmit() {
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            console.log(this.search)
            this.isEmailValid = emailRegex.test(this.search);
            
            if (!this.isEmailValid) {
                this.placeholderText = 'Please enter a valid email.';
                this.isEmailValid = false;
                this.$refs.emailInput.classList.add('invalid-email');
            }
            else {
                this.placeholderText = 'The email has been sent';
                this.isEmailValid = true          
                this.$refs.emailInput.classList.remove('invalid-email');      
                console.log('Formulario enviado:', this.search); //Forma preventiva antes de crear lo necesario para el envio al backend
            }

            this.search = ''
        }
    }
}
</script>