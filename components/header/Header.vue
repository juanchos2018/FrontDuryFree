<template>
  <div>
 <header class="header">  
    <div class="header-topbar d-none d-lg-block">
        <div class="header-topbar-inner">         
            <div class="topbar-left hidden-sm-down">
                <div class="phone"><i class="fa fa-phone left" aria-hidden="true"></i>Fono Ventas: <a href="tel:51981513145"><b>51 981513145</b></a></div>
            </div>         
            <div class="topbar-right d-flex align-items-center justify-content-end">
                <ul class="list-none">
                      <li>
                           <NuxtLink to="/Login/Login">  <i class="fa fa-lock left" aria-hidden="true"></i><span class="hidden-sm-down">Iniciar Sesión</span></NuxtLink>
                         </li>
                      <li>
                         <NuxtLink to="/Registrar/Registrar">  <i class="fa fa-lock left" aria-hidden="true"></i><span class="hidden-sm-down">Regístrate</span></NuxtLink>
                      </li>
                      <li>
                            <NuxtLink to="/Tiendas/Tiendas">  Tiendas</NuxtLink>                        
                    </li>
                    <li>
                          <NuxtLink to="/Marcas/Marcas">  MARCAS</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/Pedidos/Pedidos">PEDIDOS</NuxtLink>
                    </li>
                    <li>                        
                       <NuxtLink to="/Contactenos/Contactenos">Contáctenos</NuxtLink>
                    </li>
                </ul>
                <ul class="list-inline ml-3">
                    <li class="list-inline-item"><a href="#"><i class="fa fa-lg fa-facebook-f"></i></a></li>
                    <li class="list-inline-item"><a href="#"><i class="fa fa-lg fa-twitter"></i></a></li>
                    <li class="list-inline-item"><a href="#"><i class="fa fa-lg fa-instagram"></i></a></li>
                    <li class="list-inline-item"><a href="#" target="_blank"><i class="fa fa-lg fa-whatsapp"></i></a></li>
                </ul>
            </div>
            
        </div>
    </div>
  
    <div id="header-sticky" class="header-main">
      
        <div class="header-main-inner d-flex align-items-center">
           
            <div class="flex-grow-1 flex-lg-grow-0 mr-0 mr-lg-3">
                <div class="header-logo">           
                    <NuxtLink to="/"> 
                        <img class="" src="https://comprasentacna.com/assets/img/logo.png" alt="DPGDUTYFREE">
                  </NuxtLink>                   
                </div>
            </div>
            <div class="flex-grow-1 d-none d-lg-block">
                <div class="header-search search-form-actives">
                    <form action="/" class="d-flex" method="GET" name="site-search" role="search">
                        <div class="w-100">
                            <div class="header-search-field">
                                <input type="text" value="" id="ui_autocomplete" name="q" autocomplete="off" placeholder="¿Qué producto necesitas?" class="header-search-input ui-autocomplete-input" tabindex="0">
                            </div>
                            <div id="nav-iss-attach"></div>
                        </div>
                        <div class="flex-shrink-1">
                            <div class="header-search-submit">
                                <button type="submit" class="header-search-button" tabindex="0">
                                    <span id="spinner_loading" class="spinner-border spinner-border-sm d-none" role="status" aria-hidden="true"></span>
                                    <svg id="search_icon" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="24px" height="24px" viewBox="0 0 24 24"><g fill="none" stroke="#FFFFFF" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="11" cy="11" r="8"></circle><path d="M21 21l-4.35-4.35"></path></g></svg>
                                </button>
                            </div>
                        </div>
                    </form>
                </div>
            </div>
            <div class="ml-3">
                <div class="header-access">
                    <div class="d-flex align-items-center">
                         <NuxtLink to="/Login/Login" class="header-access-item d-flex align-items-center noselect">                      
                            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="32px" height="32px" viewBox="0 0 24 24"><g fill="none" stroke="#FFFFFF" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></g></svg>
                            <div class="my-account-block d-none d-lg-block">
                                <span class="my-account-welcome">Bienvenid@</span>
                                    <span class="my-account-user">Iniciar Sesión</span>
                                </div>                   
                        </NuxtLink>
                        <div class="header-access-item d-flex align-items-center ml-2 ml-lg-4 noselect sidebar_toggle_btn" id="sidebar_toggle_btn">
                            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="32px" height="32px" viewBox="0 0 24 24"><g fill="none" stroke="#FFFFFF" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="9" cy="21" r="1"></circle><circle cx="20" cy="21" r="1"></circle><path d="M1 1h4l2.68 13.39a2 2 0 0 0 2 1.61h9.72a2 2 0 0 0 2-1.61L23 6H6"></path></g></svg>
                            <span class="my-cart-text d-none d-lg-block">Mi Carrito</span>
                            <span class="my-cart-number">0</span>
                        </div>
                    </div>
                  </div>
            </div>
            <!-- c -->
        </div>
        <!-- inner -->
    </div>
    <!-- End Header Container -->
</header>   
  <HeaderWraper> </HeaderWraper>

  </div>
</template>

<script>

import VmMenu from '../menu/Menu';
import VmSearch from '../search/Search';
import HeaderWraper from './HeaderWraper';


export default {
    name: 'VmHeader',
   components: {
      VmSearch,
      VmMenu,
      HeaderWraper,
    
    },
    data () {
      return {
        linkedinTooltip: 'Follow us on Linkedin',
        facebookTooltip: 'Follow us on Facebook',
        twitterTooltip: 'Follow us on Twitter',
        instagramTooltip: 'Follow us on Instagram',
        isCheckoutActive: false,
        isMenuOpen: false,
         variant: 'dark',
        variants: [
          'transparent',
          'white',
          'light',
          'dark',
          'primary',
          'secondary',
          'success',
          'danger',
          'warning',
          'info',
        ]
      }
    },

   

    computed: {
      numProductsAdded () {
        return this.$store.getters.productsAdded.length;
      }
    },

    methods: {
      showCheckoutModal () {
        this.$store.commit('showCheckoutModal', true);
      },
      IniciarSesion(){

      }
    }
  };
</script>

<style lang="scss" >
 .header {
    background: #00174F;
    width: 100%;
    color: #333;
    position: relative;
    z-index: 999;
    -moz-box-shadow: 0px 0px 5px rgba(0,0,0,0.15);
    -webkit-box-shadow: 0px 0px 5px rgba(0,0,0,0.15);
    box-shadow: 0px 0px 5px rgba(0,0,0,0.15);
}

.header .header-main{
    padding-top: 10px;
    padding-bottom: 10px;
}

.header-topbar, .header-main {
    padding-left: 50px;
    padding-right: 50px;
}

.header-topbar .header-topbar-inner, .header-main .header-main-inner {
    max-width: 1820px;
    width: 100%;
    display: table;
    margin-left: auto;
    margin-right: auto;
}

 /* header a */
.header-logo{
    max-width: 250px;
}
.header-logo>a{
    display: block;
    text-decoration: none;
    outline: none;
}
.header-search{
    width: 100%;
    position: relative;
    border-radius: 5px;
    overflow: hidden;
    -webkit-border-radius: 5px;
        -moz-border-radius: 5px;
        border-radius: 5px;
}
.header-search.search-form-active, .header-search:hover{
    -webkit-box-shadow: 0 0 0 2px #0034CD, 0 0 0 3px rgba(0, 128, 255,.5);
    -moz-box-shadow: 0 0 0 2px #0034CD,0 0 0 3px rgba(0, 128, 255,.5);
    box-shadow: 0 0 0 2px #0034CD, 0 0 0 3px rgba(0, 128, 255,.5);
    z-index: 1;
}
.header-search-field{
    position: relative;
}
.header-search-input{
  width: 100%;
  border: none !important;
  height: 35px;
  padding: 5px 10px !important;
  font-size: 15px !important;
  color: #111111;
  outline: none !important;
  line-height:  35px !important;
  border-radius: 0 !important;
}
.header-search-submit{
    position: relative;
}
.header-search-button{
    position: relative;
    width: 40px;
    height: 35px;
    display: block;
    outline: none !important;
    cursor: pointer;
    background: #0034CD;
    color: #FFFFFF;
    border: none;
    border-radius: 0;
}
.header-search-button:hover{
    background: #0050E0;
}
.header-access{
    position: relative;
}
.header-access-item{
    position: relative;
    cursor: pointer;
}
a.header-access-item{
    display: block;
    text-decoration: none;
}
.header-topbar {
    display: table;
    
    color: #EEEEEE;
    width: 100%;
    font-size: 12px;
    text-transform: uppercase;
    letter-spacing: 0.4px;
}

    .header-topbar .topbar-left {
        text-align: left;
        display: table-cell;
        vertical-align: middle;
    }

    .header-topbar .topbar-left .phone a{
        color: #EEEEEE;
    }

    .header-topbar .topbar-left .phone a:hover{
        color: #000000;
    }

    .header-topbar .topbar-right {
        text-align: right;
        display: table-cell;
        vertical-align: middle;
    }

        .header-topbar .topbar-right ul li {
            text-align: left;
            display: inline-block;
        }

        .header-topbar .topbar-right > ul > li > a {
            margin-top: 0;
            margin-right: 0;
            margin-bottom: 0;
            margin-left: 8px;
            margin-right: 8px;
            padding-top: 10px;
            padding-bottom: 10px;
            display: block;
            color: #EEEEEE;
        }


        .header-topbar .topbar-right ul li a:hover {
            color: #000000
        }

        .header-topbar .topbar-right > ul > li:last-child > a {
            margin-right: 0px;
        }

@media only screen and (max-width: 420px) {
    .header-main .logo {
        display: block;
        margin: 30px auto 10px;
        width: 100%;
        float: none;
    }

        .header-main .logo a {
            margin: 0 auto !important;
        }

    .sidebar-icon-nav ul li {
        margin: 20px 12px !important;
    }

    .header-access-item>svg{
        width: 28px;
        height: 28px;
    }
}
.my-account-block{
    color: #FFFFFF;
    line-height: 15px;
    margin-left: 5px;
}
.my-account-welcome{
    font-weight: 400;
    display: block;
}
.my-account-user{
    display: block;
    font-weight: 700;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    max-width: 100px;
}

.my-cart-text{
    color: #FFFFFF;
    font-weight: 700;
    margin-left: 10px;
}
.my-cart-number{
    background: #ee4130 none repeat scroll 0 0;
    color: #FFFFFF;
    font-size: 13px;
    font-weight: 400;
    line-height: 18px;
    padding: 0;
    position: absolute;
    left: 20px;
    top: -7px;
    width: 20px;
    height: 20px;
    text-align: center;
    border-radius: 50%;
}



// header wraper
.header_wrap {
	transition: all 0.5s ease 0s;
}
.header_wrap:not([class*="bg_"]):not([class*="bg-"]) {
	background-color: #fff;
}
.header_wrap:not([class*="bg_"]):not([class*="bg-"]).transparent_header {
	background-color: transparent;
}
.header_wrap:not([class*="bg_"]):not([class*="bg-"]).transparent_header.nav-fixed {
	background-color: #fff;
}
.header_wrap:not([class*="bg_"]):not([class*="bg-"]).transparent_header.light_skin.nav-fixed,
.header_wrap:not([class*="bg_"]):not([class*="bg-"]).transparent_header.nav-fixed .light_skin {
	background-color: #1D2224;
}
.header_wrap:not([class*="bg_"]):not([class*="bg-"]).transparent_header.sticky_dark_skin.nav-fixed,
.light_skin .sidetoggle_icon::after,
.light_skin .sidetoggle_icon::before,
.light_skin .toggle_center_line {
	background-color: #fff;
}

nav-dropdown .new-label, .nav-dropdown .sale-label {
    padding: 2px 4px;
    font-size: 10px;
    text-transform: uppercase;
    font-weight: 400;
    margin-left: 5px;
    border-radius: 2px;
    -moz-border-radius: 2px;
    -webkit-border-radius: 2px;
}

.nav-dropdown .sale-label {
    background: #f55151;
    color: #fff;
}

.nav-dropdown .new-label {
    background: #00174F;
    color: #fff;
}

.nav-dropdown .sub-banner {
    padding: 0;
    position: relative;
    width: 100%;
    border: 0 none;
}

.nav-main-grid{
    width: 100%;
    position: relative;
}
.nav-main-grid .navmain-g-ul{
    margin: 0;
    padding: 0;
}
.nav-main-grid .navmain-g-ul>li{
    font-size: 14px;
    text-transform: none;
    color: #333;
    font-weight: 400;
}
.nav-main-grid .navmain-g-ul>li>a{
    color: #222222;
    font-weight: 400;
    font-size: 14px;
    padding-top: 2px;
    padding-left: 0px;
    padding-right: 0px;
    padding-bottom: 2px;
    display: inline-block;
    transition: all 0.2s ease 0s;
    -moz-transition: all 0.2s ease 0s;
    -o-transition: all 0.2s ease 0s;
    -webkit-transition: all 0.2s ease 0s;
    border: 0 !important;
}

.nav-main-grid .navmain-g-ul > li:hover > a {
    color: inherit;
}

.nav-main-grid .navmain-g-ul > li > a:hover {
    padding-left: 5px;
    color: #00174F;
}
.navbar-nav .dropdown-menu {
	border: 0;
	border-radius: 0;
	margin: 0;
	padding: 0;
	min-width: 14rem;
}
.navbar-nav .dropdown-menu {
	background-color: #252A2C;
}
.mega-menu {
	display: table;
	padding: 15px 0;
	width: 100%;
	-ms-flex-wrap: wrap;
	flex-wrap: wrap;
}
.mega-menu ul {
	-ms-flex-wrap: wrap;
	flex-wrap: wrap;
}
.menu_banners {
	display: block;
}

.header_banner_wrap {
	padding: 15px;
	height: 100%;
}
.header-banner2 {
	margin: 0 15px;
}
.header-banner,
.header-banner2 {
	display: block;
	position: relative;
	margin-bottom: 15px;
}

.mega-menu-col {
	border-right: 1px solid #ddd;
	padding: 0;
}
.mega-menu-col:last-child {
	border-right: 0 !important;
}

.dropdown-menu li a i {
    font-size: 14px;
    width: 20px;
    display: inline-block;
	vertical-align: middle;
}
.navbar .navbar-nav li.dropdown-mega-menu {
	position: static;
}
.navbar .navbar-nav li.dropdown-mega-menu .dropdown-menu {
	right: 0;
	padding-left: 0;
    padding-right: 0;
    border: 1px solid #ddd;
}

.dark_skin .mega-menu-col, .dark_skin .cart_list li {
    border-color: #ddd;
}
</style>
