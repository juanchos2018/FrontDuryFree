<template>
    <div>
        <section class="section-default py-5">
    <div class="container-lg">
        <div class="row">
            <div class="col-sm-12 col-md-12 col-lg-4 mt-3 mb-3">
                <div class="contact-head">
                    <p class="contact-head__text font-title font-900">Contáctenos aquí y estaremos encantados de responder sus consultas generales.</p>
				</div>
            </div>
            <div class="col-sm-12 col-md-12 col-lg-8 mt-3 mb-3">
                                <div class="contact-form">
						<!-- form -->
						<form role="form" name="FormOrders" id="FormOrders" action="https://comprasentacna.com/pedidos" method="POST" enctype="multipart/form-data">
							<div class="form-row">
								<div class="form-group col-sm-12 col-md-12 col-lg-12">
									<input type="text" name="name" id="name" class="form-control form-control-lg" placeholder="Nombre" required="" data-error="Por favor, escriba su nombre">
									<div class="help-block with-errors"></div>
								</div>
								<div class="form-group col-sm-6 col-md-6 col-lg-6">
									<input type="email" name="email" id="email" class="form-control form-control-lg" placeholder="Correo electrónico" required="" data-error="Por favor introduzca su correo electrónico">
									<div class="help-block with-errors"></div>
								</div>
								<div class="form-group col-sm-6 col-md-6 col-lg-6">
									<input type="text" name="phone" id="phone" class="form-control form-control-lg" placeholder="Teléfono" required="" data-error="Por favor introduzca su teléfono">
									<div class="help-block with-errors"></div>
								</div>
								<div class="form-group col-sm-12 col-md-12 col-lg-12">
									<input type="text" name="subject" id="subject" class="form-control form-control-lg" placeholder="Asunto" required="" data-error="Por favor ingrese su asunto del mensaje">
									<div class="help-block with-errors"></div>
								</div>
								<div class="form-group col-sm-12 col-md-12 col-lg-12">
                                    <label>Archivos PDF o WORD</label>
									<input type="file" name="file" id="file" class="form-control" placeholder="Archivo" required="">
									<div class="help-block with-errors"></div>
								</div>
								<div class="form-group col-sm-12 col-md-12 col-lg-12">
									<textarea rows="6" name="message" id="message" class="w-100" placeholder="Mensaje" required="" data-error="Escribe tu mensaje"></textarea>
									<div class="help-block with-errors"></div>
								</div>
							</div>
							<div class="form-group">
                                <button class="button  is-rounded" style="background:#00174f;color:#FFFFFF">ENVIAR</button>     
							</div>
						</form>
						<!-- form -->
				</div>
            </div>
        </div>
    </div>
</section>
    </div>
</template>

<script>
export default {
    
}
</script>