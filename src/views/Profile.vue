<template>

    <div class="holder">
                <Navbar/>

        <div class="container">
        <section id="personal" class="mt-4 py-3">
            <form class="form">
                <h1 class="" style="color:black; font-weight: bold;">Personal Information</h1>
                <div class="row">
                    <div class="col-md-6 my-3">
                        <div class="input-group">
                            <input type="text" class="form-control shadow-none" placeholder="First Name">
                        </div>
                    </div>
                    <div class="col-md-6 my-3">
                        <div class="input-group">
                            <input type="text" class="form-control shadow-none" placeholder="Last Name">
                        </div>
                    </div>
                    <div class="col-md-6 my-3">
                        <div class="input-group">
                            <input type="text" class="form-control shadow-none" placeholder="Other Names">
                        </div>
                    </div>
                    <div class="col-md-6 my-3">
                        <div class="input-group">
                            <input type="number" class="form-control shadow-none" placeholder="Age">
                        </div>
                    </div>
                    <div class="col-md-12 my-3">
                        <div class="input-group">
                            <input type="submit" class="btn btn-primary" value="Save">
                        </div>
                    </div>
                    
                </div>
                

            </form>
            
        </section>

        <section id="location" class="mt-4 py-3">
            <form class="form">
                <h1 class="" style="color:black; font-weight: bold;">Location Information</h1>
                <div class="row">
                    <div class="col-md-6 my-3">
                        <div class="input-group">
                            <input type="text" class="form-control shadow-none" placeholder="Country">
                        </div>
                    </div>
                    <div class="col-md-6 my-3">
                        <div class="input-group">
                            <input type="text" class="form-control shadow-none" placeholder="State">
                        </div>
                    </div>
                    <div class="col-md-4 my-3">
                        <div class="input-group ">
                            <input type="text" class="form-control shadow-none" placeholder="LGA">
                        </div>
                    </div>
                    <div class="col-md-8 my-3">
                        <div class="input-group">
                            <input type="text" class="form-control shadow-none" placeholder="Address">
                        </div>
                    </div>
                    <div class="col-md-12 my-3">
                        <div class="input-group">
                            <input type="submit" class="btn btn-primary" value="Save">
                        </div>
                    </div>
                </div>
                

            </form>
            
        </section>

        </div> 
    </div>
</template>

<script>
import Navbar from '../components/Navbar.vue'

export default {
    name : 'Profile',
    components : {
    Navbar,
    
}
    
}
</script>

<style lang="scss" scoped>
.form{
    width: 100%;
    // background-color: red;
    border: 1px solid black;
    padding: 30px;
}
.input-group input{
    padding: 18px;
}
.holder{
    min-height: 120vh;
    width: 100%;
    background-image: linear-gradient(rgb(192, 226, 246),rgb(248, 194, 203));
}
</style>