<template>
    <div class="holder">
        <form class="form" id="register-form">
            <h2 class="register-text mb-4">REGISTER</h2>
            <!-- <div class="input-group">
                <input type="text" class="form-control shadow-none py-3" placeholder="Firstname">
            </div>
            <div class="input-group my-3">
                <input type="text" class="form-control shadow-none py-3" placeholder="Lastname">
            </div> -->
            <div class="input-group my-3">
                <input type="text" class="form-control shadow-none py-3" placeholder="Username">
            </div>
            <div class="input-group my-3">
                <input type="password" class="form-control shadow-none py-3" placeholder="Password">
            </div>
            <div class="input-group my-3">
                <input type="password" class="form-control shadow-none py-3" placeholder="Confirm Password">
            </div>
            <div class="input-group my-3">
                <input type="submit" value="Register" class="btn btn-primary" id="submitBtn">
            </div>
            <p class="text-center" style="font-weight: bold;">Already have an account? <router-link to="/login" style="text-decoration:none; color:white;">Login</router-link></p>

        </form>
    </div>
</template>

<script>
export default {
    name : 'Register'
}
</script>

<style lang="scss" scoped>
.holder{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    background-image: linear-gradient(rgb(188, 200, 223), rgb(45, 126, 238));
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
.register-text{
    color: white !important;
    text-align: center;
}
#submitBtn{
    margin: 0 auto;
    padding: 10px 20px;
    width: 100% !important;
}
</style>