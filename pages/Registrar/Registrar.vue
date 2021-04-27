<template>
    <div>
    <section class="content-page">
    <div class="container-lg">
        <br>
        <br>
        <div class="row">
            <div class="col-md-6">
                <div class="form-border-box">
                    <form method="POST">
                        <h2 class="normal"><span>Crear Cuenta</span></h2>                       
                       <b-form-group
                        id="input-group-1"
                        label="Nombres"
                        label-for="input-1"              
                                >
                        <input class="input is-normal" type="text" placeholder="Normal input">
                    </b-form-group>
                    <div class="form-row">                         
                      <b-form-group
                        id="input-group-1"
                        label="Fecha de nacimiento"
                        label-for="input-1"  
                        class="col-md-6"     
                                >
                           <input class="input is-normal" type="date" placeholder="Normal input">
                    </b-form-group>
                     <b-form-group
                        id="input-group-1"
                        label="Género"
                        label-for="input-1"  
                       class="col-md-6"         
                                >
                      <div class="select is-primary" >
                                <select style="width:100%">
                                     <option value="H">Masculino</option>
                                    <option value="M">Femenino</option>
                                </select>
                                </div>
                    </b-form-group>
                    </div>
                     

                    <b-form-group
                        id="input-group-1"
                        label="Correo electrónico"
                        label-for="input-1"  
                        class="form-field-wrapper"     
                                >
                            <input class="input is-normal" type="eamil" placeholder="Normal input">
                    </b-form-group>


                        
                    <b-form-group
                        id="input-group-1"
                        label="Contraseña"
                        label-for="input-1"  
                        class="form-field-wrapper"     
                                >
                      <input class="input is-normal" type="password" >
                    </b-form-group>
                <b-form-group
                        id="input-group-1"
                        label="Repetir Contraseña"
                        label-for="input-1"  
                        class="form-field-wrapper"     
                                >
                      <input class="input is-normal" type="password" >
                    </b-form-group>


                        <div class="form-field-wrapper">
                            <input type="hidden" name="_token" value="r18L9afg3jUqHk0Bx6py8Tve3NQjLrmPIduwpV5B">
                              <button class="button  is-rounded" style="background:#00174f;color:#FFFFFF">REGISTRARME</button>     
                        </div>
                    </form>

                </div>
            </div>
                        

            <div class="col-md-6">
                <div class="form-border-box">
                    <div>
                        <h2 class="normal"><span>¿Ya tienes una Cuenta?</span></h2>
                        <p>Inicia sesion y desfrutaras de una experiencia de compra mas rapida.</p>
                        <div class="form-field-wrapper">                        
                        <NuxtLink to="/Login/Login" class="button is-black is-rounded"> INICAR SESION</NuxtLink>
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