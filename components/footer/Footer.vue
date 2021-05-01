<template>
  <div class="footer">
    
   <section class="section-default section-infof py-4 border-bottom-f">
    <div class="container-lg">
        <div class="row">
            <div class="col-12 col-sm-12 col-md-6 col-lg-4 my-3">
                <div class="info-item">
                    <div class="info-item_icon"><i class="fa fa-calendar-check-o"></i></div>
                    <div class="info-item_content">
                        <h5 class="info-item_title mb-2">Horarios de Atención</h5>
                        <p class="info-item_description">Lunes a Viernes 09:00 - 19:00</p>
                        <p class="info-item_description">Sábados 10:00 - 18:00</p>
                    </div>
                </div>
            </div>
            <div class="col-12 col-sm-12 col-md-6 col-lg-4 my-3">
                <div class="info-item">
                    <div class="info-item_icon"><i class="fa fa-whatsapp"></i></div>
                    <div class="info-item_content">
                        <h5 class="info-item_title mb-2">Venta por WhatsApp</h5>
                        <p class="info-item_description">51 981513145 (Solo Whatsapp, no llamadas)</p>
                        <p class="info-item_description">Lunes a Viernes 09:00 - 19:00</p>
                    </div>
                </div>
            </div>
            <div class="col-12 col-sm-12 col-md-6 col-lg-4 my-3">
                <div class="info-item">
                    <div class="info-item_icon"><i class="fa fa-phone"></i></div>
                    <div class="info-item_content">
                        <h5 class="info-item_title mb-2">Servicio al Cliente</h5>
                        <p class="info-item_description">Teléfono: (052) 578214</p>
                        <p class="info-item_description">ventas@dpgdutyfree.com</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
    
  <div class="w-100 pt-5 pb-4">
        <div class="container-lg">
            <div class="row">
                <div class="col-lg-3 col-md-12 col-sm-12 mb-sm-45">
                    <div class="footer-block about-us-block">
                        <img src="https://comprasentacna.com/assets/img/logo-white.png" class="img-fluid" alt="">
                        <p>DPG, es una empresa con más de 35 años de experiencia en la distribución y retail de las marcas de lujo más reconocidas a nivel mundial.</p>
                        <ul class="footer-social-icon list-none-ib">
                            <li><a href="#" ><i class="fa fa-facebook" aria-hidden="true"></i></a></li>
                            <li><a href="#" ><i class="fa fa-twitter" aria-hidden="true"></i></a></li>
                            <li><a href="#" ><i class="fa fa-instagram" aria-hidden="true"></i></a></li>
                            <li><a href="#" ><i class="fa fa-whatsapp" aria-hidden="true"></i></a></li>
                        </ul>
                    </div>
                </div>
                <div class="col-lg-2 col-md-4 col-sm-6 mb-sm-45">
                    <div class="footer-block information-block">
                        <h6 class="text-uppercase">Información</h6>
                        <ul>
                            <li><a href="#">Sobre Nosotros</a></li>
                            <li><a href="#">Términos y Condiciones</a></li>
                           
                            <li><a href="#">Cambios y Devoluciones</a></li>
                            <li><a href="#">Contacte con Nosotros</a></li>
                        </ul>
                    </div>
                </div>
                <div class="col-lg-2 col-md-4 col-sm-6 mb-sm-45">
                    <div class="footer-block links-block">
                        <h6 class="text-uppercase">Enlaces</h6>
                        <ul>
                            <li><a href="#">Iniciar Sesión</a></li>
                            <li><a href="#">Regístrate</a></li>
                            <li><a href="#">Pedidos</a></li>
                            <li><a href="#">Marcas</a></li>
                            
                        </ul>
                    </div>
                </div>
                <div class="col-lg-2 col-md-4 col-sm-6 mb-sm-45">
                    <div class="footer-block extra-block">
                        <h6 class="text-uppercase">Productos</h6>
                        <ul>
                            <li><a href="#">Perfumería</a></li>
                            <li><a href="#">Licores</a></li>
                            <li><a href="#">Lentes</a></li>
                            <li><a href="#">Relojes</a></li>
                           
                        </ul>
                    </div>
                </div>
                <div class="col-lg-3 col-md-12 col-sm-6">
                    <div class="footer-block contact-block">
                        <h6 class="text-uppercase">Contacto</h6>
                        <ul>
                            
                            <li><i class="fa fa-envelope" aria-hidden="true"></i><a href="#">ventas@dpgdutyfree.com</a></li>
                            <li><i class="fa fa-phone" aria-hidden="true"></i><a href="#">(052) 578214</a></li>
                            <li><i class="fa fa-whatsapp" aria-hidden="true"></i><a href="#" target="_blank">51 981513145</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'VmFooter',
}
</script>

<style lang="scss" scoped>
.footer {
    background: #00174F;
}
.border-bottom-f {
    border-bottom: 1px solid rgba(255, 255, 255, 0.25);
}
.section-infof {
    width: 100%;
    position: relative;
    background: #00174F;
}
.mb-3, .my-3 {
    margin-bottom: 1rem !important;
}
.info-item {
    position: relative;
    text-align: center;
}
.info-item_icon i {
    color: #FFFFFF;
    font-size: 2em;
}
.info-item_title {
    font-weight: 700;
    font-size: 16px;
    color: #FFFFFF;
    margin: 0;
}

.info-item_description {
    margin: 0;
    color: #EEEEEE;
}
.footer-block {
    display: block;
    margin: 0;
}
.img-fluid {
    max-width: 100%;
    height: auto;
}
.footer-block p {
    color: #EEEEEE;
    margin: 30px 0;
}
ul.list-none-ib li, .list-none-ib {
    display: inline-block;
}
.footer-block ul li a {
    color: #EEEEEE;
    margin: 0 auto;
}
.footer-social-icon li a {
    background: rgba(255, 255, 255, 0.13) none repeat scroll 0 0;
    border-radius: 50px;
    color: #ffffff !important;
    display: inline-block;
    height: 40px;
    line-height: 40px;
    text-align: center;
    width: 40px;
    text-align: center;
}
.footer-block h6 {
    color: #fff;
    margin-bottom: 30px;
}

.footer-block.contact-block li i {
    position: absolute;
    left: 0;
    line-height: inherit;
}
.fa {
    display: inline-block;
    font: normal normal normal 14px/1 FontAwesome;
    font-size: inherit;
    text-rendering: auto;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}
ol, ul {
    margin: 0;
    padding: 0;
}
ul {
    display: block;
    list-style-type: disc;
    margin-block-start: 1em;
    margin-block-end: 1em;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
    padding-inline-start: 40px;
}
p {
    font-weight: 400;
    font-size: 14px;
    font-family: 'Open Sans', sans-serif;
    color: #444444;
}
</style>
