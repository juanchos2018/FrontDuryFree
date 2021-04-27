<template>
    
        <section class="section-padding-sm promo">
    <div class="container-lg">
        <div class="promo-box row">
            <div class="col-md-4 mtb-sm-30 promo-item">
                <div class="icon d-block"></div>
                <div class="info text-center">
                    <i class="fa fa-truck x-2" aria-hidden="true"></i>
                    <br>
                    <h6 class="font-title">Despacho a Todo Tacna</h6>
                    <p>Rápido y a domicilio u oficina de transporte.</p>
                </div>
            </div>
            <div class="col-md-4 mtb-sm-30 promo-item">
                <div class="icon d-block"></div>
                <div class="info text-center">
                    <i class="fa fa-shopping-basket" aria-hidden="true"></i>
                    <br>
                    <h6 class="font-title">Retiro Sin Costo</h6>
                    <p>Compra online y retira gratis en cualquier tienda DPG Duty Free.</p>
                </div>
            </div>
            <div class="col-md-4 mtb-sm-30 promo-item">
                <div class="icon d-block"></div>
                <div class="info text-center">
                    <i class="fa fa-smile-o" aria-hidden="true"></i>
                    <br>
                    <h6 class="font-title">Cambios Y Devoluciones</h6>
                    <p>En DPG Duty Free cambiar de opinión no es un problema.</p>
                </div>
            </div>
        </div>
    </div>
</section>
    
</template>

<script>
export default {
      name: 'Promo',
}
</script>

<style lang="scss">
.container-lg {
    max-width: 960px;
}

.section-padding-sm {
    padding-bottom: 40px;
    padding-top: 40px;
}
.promo {
    position: relative;
}
.promo-box .promo-item {
    text-align: center;
    border-right: 1px solid #eee;
}
.promo-box {
    background: #ffffff none repeat scroll 0 0;
    /* border: 1px solid #eeeeee; */
    padding: 10px 0px;
    position: relative;
    width: 100%;
}
.promo-box .promo-item {
    text-align: center;
    border-right: 1px solid #eee;
}
.promo-box .icon {
    display: inline-table;
    vertical-align: middle;
}
.fa {
    display: inline-block;
    font: normal normal normal 14px/1 FontAwesome;
    font-size: inherit;
    text-rendering: auto;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}
.row {
    display: -ms-flexbox;
    display: flex;
    -ms-flex-wrap: wrap;
    flex-wrap: wrap;
    margin-right: -15px;
    margin-left: -15px;
}
</style>