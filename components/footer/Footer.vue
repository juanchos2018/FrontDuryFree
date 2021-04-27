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
</style>
