<template>
  <div>

 <div class="owl-item active" style="width: 290px; margin-right: 30px;"><div class="product-item d-flex flex-column h-100">
                        <div class="product-item-inner">
                            <div class="product-img-wrap">
                              <nuxt-link
                                class="details"
                                :to="{
                                  name: 'product_detail-id',
                                  params: {
                                    id: product.id,
                                    title: product.title,
                                    price: product.price,
                                    rating: product.ratings,
                                    reviews: product.reviews,
                                    isAddedBtn: product.isAddedBtn
                                  }
                                }"
                              >
                              </nuxt-link>
                              <img src="perfume1.jpg" alt="212 VIP 80 ML EDP DAMA">
                            </div>
                        <!--    <span class="label_discount text-nowrap">10%OFF</span>-->
                     <span class="label-stock stock_available text-nowrap">En stock</span>
                        </div>
                        <div class="product-detail d-flex flex-column flex-grow-1">
                          <div class="product-rating">
                                <div class="star-rating" itemprop="reviewRating" itemscope="" itemtype="#" title="Rated 0 out of 5">
                                    <span style="width: 0%"></span>
                                </div>
                            </div>
                            <div>
                                <p class="product-title product-line-clamp"><a href="#">{{ product.title }}</a></p>
                            </div>
                            <div class="mt-auto">
                                <div>
                                    <a class="tag" href="#">PERFUMERIA</a>
                                    <div class="rg_productviews-list">.</div>
                                    <h5 class="item-price">
                                    <del>S/ 289.00</del>
                                  S/   {{ product.price }}</h5>
                                </div>
                                <div class="product-addtocart w-100 d-flex mt-auto pt-2 px-1">
                                    <div class="count-input-box mr-1">
                                        <div class="count-input-block">
                                            <input class="form-control quantity_input" min="1" max="5" type="text" value="1">
                                            <div class="count-input-btns">
                                                <button class="inc-amount count-btn"><i class="fa fa-chevron-up"></i></button>
                                                <button class="dec-amount count-btn"><i class="fa fa-chevron-down"></i></button>
                                            </div>
                                        </div>
                                    </div>
                                    <button type="button" class="btn-add-to-cart add_to_cart d-flex align-items-center" data-qty="1" data-code="2" @click="showCheckoutModal()">
                                        <span class="spinner-loading spinner-border spinner-border-sm d-none mr-2" role="status" aria-hidden="true"></span>
                                        <img width="20px" class="p-icon-cart" src="https://comprasentacna.com/assets/img/icons/cart.svg">
                                        <span>Añadir al Carrito</span>
                                    </button>
                                  </div>
                        </div>
               </div>
         </div>
 </div>
  
  </div>
</template>

<script>
export default {
  name: 'products',
  props: ['product'],

  data () {
    return {
      addToCartLabel: 'Agregar Carro',
      viewDetailsLabel: 'Details',
      removeFromCartLabel: 'Remove from cart',
      addToFavouriteLabel: 'Add to favourite',
      removeFromFavouriteLabel: 'Remove from favourite',
      selected: 1,
      quantityArray: []
    }
  },

  mounted () {
    for (let i = 1; i <= 20; i++) {
      this.quantityArray.push(i);
    }

    if (this.$props.product.quantity > 1) {
      this.selected = this.$props.product.quantity;
    }
  },

  computed: {
    isUserLogged () {
      return this.$store.getters.isUserLoggedIn;
    }
  },

  methods: {
     showCheckoutModal () {     
        this.$store.commit('showAddModal', true);
      },
    addToCart (id) {
      let data = {
        id: id,
        status: true
      }
      this.$store.commit('addToCart', id);
      this.$store.commit('setAddedBtn', data);
    },
    removeFromCart (id) {
      let data = {
        id: id,
        status: false
      }
      this.$store.commit('removeFromCart', id);
      this.$store.commit('setAddedBtn', data);
    },
    saveToFavorite (id) {
      let isUserLogged = this.$store.state.userInfo.isLoggedIn;

      if (isUserLogged) {
        this.$store.commit('addToFavourite', id);
      } else {
        this.$store.commit('showLoginModal', true);
      }
    },
    removeFromFavourite (id) {
      this.$store.commit('removeFromFavourite', id);
    },
    onSelectQuantity (id) {
      let data = {
        id: id,
        quantity: this.selected
      }
      this.$store.commit('quantity', data);
    }
  }
}
</script>

<style lang="scss" scoped>
 .details {
    cursor: pointer;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 1;

    &:hover {
      border: 1px solid #51bafc;
    }
 }
 .button,
 .select {
   z-index: 2;
 }
 .select {
   position: absolute;
   right: 15px;
   bottom: 35px;
 }
 .card-content {
   padding: 0;
 }
 .buttons {
   margin: 0;
 }
.product-addtocart .count-input-block .count-input-btns {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
      -ms-flex-direction: column;
          flex-direction: column;
  margin-left: -1px;
}

.product-addtocart .count-input-block .count-input-btns .count-btn {
  background: #FFFFFF;
  padding: 0 5px;
  border: 1px solid #CCCCCC;
  height: 20px;
  font-weight: 400;
  outline: none;
  border-radius: 0 !important;
}

.product-addtocart .count-input-block .count-input-btns .count-btn i {
  font-size: 10px;
  line-height: 20px;
  color: #000000;
  margin: auto;
}

.product-addtocart .count-input-block .count-input-btns .count-btn:hover {
  background: #00174F;
}
.product-addtocart .count-input-block .count-input-btns .count-btn:hover i{
    color: #FFFFFF;
}

.product-addtocart .count-input-block .count-input-btns .count-btn + .count-btn {
  border-top: none;
}
</style>


