<template>
    <div class="container newsl_container">
        <h2>Join to our newsletter</h2>
        <div class="form">
            <input type="text" v-model="email"/>
            <button @click="submitHandler">Subscribe</button>
        </div>
        <div class="small">
            <p>xxxx</p>
        </div>
        <div class="error_label">
            <div>{{error}}</div>
        </div>
        <div class="success_label">
            <div>{{success}}</div>
        </div>

    </div>
</template>

<script>
    export default {
        data(){
            return {
                email:'',
                error:'',
                success:''
            }
        },
        methods:{
            validate(email){
                let valid = [true, '']

                if(!/\S+@\S+\.\S+/.test(email)){
                    valid = [false, 'Enter a valid email']
                }
                if(email === ''){
                    valid = [false, 'It is empty']
                }
                return valid
            },
            submitHandler(){
                let valid = this.validate(this.email)

                if(valid[0]){
                    this.error = '';
                    this.addEmail(this.email)
                } else {
                    this.error = valid[1]
                }
            },
      //      addEmail(email){}
        
        }
    }
</script>