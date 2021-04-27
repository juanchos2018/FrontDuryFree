<template>
    <div>
    <section class="content-page">
    <div class="container-lg">
        <br>
        <br>
        <div class="row">
            <div class="col-md-6">
                <div class="form-border-box">
                   <b-form  v-if="show">
                   <h2 class="normal"><span>Ingrese a su cuenta</span></h2>
                    <b-form-group
                        id="input-group-1"
                        label="Corre Electronico:"
                        label-for="input-1"
              
                    >
                        <b-form-input
                        id="input-1"
                        v-model="form.email"
                        type="email"
                        placeholder="Enter email"
                        required
                        ></b-form-input>
                    </b-form-group>

                    <b-form-group id="input-group-2" label="Contraseña:" label-for="input-2">
                        <b-form-input
                        id="input-2"
                        v-model="form.name"
                        placeholder="Enter name"
                        required
                        ></b-form-input>
                    </b-form-group>
                  <button class="button  is-rounded" style="background:#00174f;color:#FFFFFF">INICIAR SESION</button>     
            
                </b-form>
                </div>
            </div>
            <div class="col-md-6">
                <div class="form-border-box">
                    <div>
                        <h2 class="normal"><span>¿No estás registrado?</span></h2>
                        <p>Regístrate en nuestro sitio y descubre todas las oportunidades que tenemos para ti.</p>
                        <div class="form-field-wrapper">
                        
                               <NuxtLink to="/Registrar/Registrar" class="button is-black is-rounded"> CREAR UNA CUENTA</NuxtLink>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
<br>
<br>
    </div>
</template>


<script>
export default {
    data(){
        return{
              form: {
            email: '',
            name: '',
            food: null,
            checked: []
            },
            foods: [{ text: 'Select One', value: null }, 'Carrots', 'Beans', 'Tomatoes', 'Corn'],
            show: true
        }
    }
}
</script>

<style lang="scss" >

.form-border-box {
    border: 1px solid #eee;
    padding: 30px;
}

</style>