<template>
    <footer>
        <div class="container">
                <img :src="logoIcon"/>
                <div class="contact">
                    <div>Call us</div>
                    <div>4566-7789</div>
                </div>
        </div>
    </footer>
</template>

<script>
    import Logo from '../../assets/images/logo.png';

    export default {
        data(){
            return {
                logoIcon: Logo
            }
        }
    }
</script>