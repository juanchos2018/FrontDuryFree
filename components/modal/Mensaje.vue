<template>
    <div :class="[ openModal ? 'is-active' : '', 'modal' ]">>
        <div class="modal-dialog modal-dialog-centered modal-sm" id="cart_added_message">
			<div class="modal-content modal-product-added py-2">
        <button type="button" class="modal-added-close close" data-dismiss="modal" aria-label="Close" @click="closeModal(false)"><span aria-hidden="true">×</span></button>
        <div class="modal-body">
        <i class="fa fa-check"></i>
        <p class="modal-product-added-message">Producto agregado<br> al Carrito</p>
        <div class="modal-product-added-actions">
            
			 <NuxtLink to="/Carrito/MiCarrito" class="button  is-rounded" style="background:#00174f;color:#FFFFFF"> Ir al Carrito</NuxtLink>
 
				 <NuxtLink to="/" class="button is-rounded is-primary is-outlined" > Pasar por Caja</NuxtLink> <br>
            <a href="#" onclick="return false" data-dismiss="modal" class="btn-added-light">Seguir comprando</a>
        </div>
    </div>
</div></div>
    </div>
</template>
<script>

export default {
	name: 'checkout',
    
	data () {
		return {
			modalTitle: 'Checkout',
			removeLabel: 'Remove from cart',
			cartEmptyLabel: 'Your cart is empty',
			closeLabel: 'Close',
			isCheckoutSection: false
		}
	},

	computed: {
			products () {
				return this.$store.getters.productsAdded;
			},
			openModal () {
				if (this.$store.getters.isAddModalOpen) {
					return true;
				} else {
					return false;
				}
			},			
			isUserLoggedIn () {
				return this.$store.getters.isUserLoggedIn;
			}
	},

	methods: {
		closeModal (reloadPage) {
			this.$store.commit('showAddModal', false);

			if (reloadPage) {
				window.location.reload();
			}
		},
	
		onPrevBtn () {
			this.isCheckoutSection = false;
		}
	}
}
</script>
<style lang="scss" scoped>
.modal.show .modal-dialog {
    -webkit-transform: none;
    transform: none;
}
.modal-body {
    position: relative;
    -ms-flex: 1 1 auto;
    flex: 1 1 auto;
    padding: 1rem;
}
.modal-product-added-actions {
    text-align: center;
}
.modal-product-added-message {
    font-weight: 700;
    font-size: 15px;
    color: #54b268;
    margin-bottom: 20px;
    margin-top: 10px;
    text-align: center;
}
.modal-product-added .fa-check {
    background: #54b268;
    color: #fff;
    width: 60px;
    height: 60px;
    border-radius: 100%;
    line-height: 60px;
    display: block;
    margin: 0 auto;
    font-size: 30px;
    text-align: center;
}
button.close {
    padding: 0;
    background-color: transparent;
    border: 0;
}
.modal-added-close {
    position: absolute;
    right: 5px;
    top: 0;
    z-index: 99;
    outline: none !important;
    padding: 0;
}
.modal.fade .modal-dialog {
    transition: -webkit-transform 0.3s ease-out;
    transition: transform 0.3s ease-out;
    transition: transform 0.3s ease-out, -webkit-transform 0.3s ease-out;
    -webkit-transform: translate(0, -50px);
    transform: translate(0, -50px);
}
</style>

