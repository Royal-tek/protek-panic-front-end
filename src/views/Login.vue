<template>
    <div class="holder">
        <form class="form" id="login-form">
            <h2 class="login-text mb-4">LOGIN</h2>
            <div class="input-group">
                <input type="text" class="form-control shadow-none py-3" placeholder="Username">
            </div>
            <div class="input-group my-3">
                <input type="password" class="form-control shadow-none py-3" placeholder="Password">
            </div>
            <div class="input-group my-3">
                <input type="submit" class="btn btn-primary" id="submitBtn">
            </div>
            <p class="text-center" style="text-decoration:none; font-weight: bold;">Don't have an account? <router-link to="/register" style="text-decoration:none; color:white;">Register</router-link></p>


        </form>
    </div>
</template>

<script>
export default {
    name : 'Login'
}
</script>

<style lang="scss" scoped>
.holder{
    display: flex;
    align-items: center;
    justify-content: center;
    background-image: linear-gradient(rgb(188, 200, 223), rgb(45, 126, 238));
    width: 100%;
    height: 100vh;
    }
.form{
    width: 30%;
    border-radius: 20px;
    padding: 50px 10px;
    background-color: rgb(111, 111, 183) !important;
}
.input-group{
    width: 80%;
    margin: 0 auto;
}
.login-text{
    color: white !important;
    text-align: center;
}
#submitBtn{
    margin: 0 auto;
    padding: 10px 20px;
    width: 100% !important;
}
</style>