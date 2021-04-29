<template>
  <div>
    <VmHero></VmHero>
    <Promo></Promo>

    <VmProductsList></VmProductsList>
    <br>
   <Categoria></Categoria>

  </div>
</template>

<script>
import VmProductsList from '@/components/products_list/ProductsListContainer';
import VmHero from '@/components/hero/Hero';
import Promo from '@/components/promo/Promo'
import Categoria from '@/components/categoria/Categoria'
import 'bootstrap/dist/css/bootstrap.css' 
import 'bootstrap-vue/dist/bootstrap-vue.css'
export default {
  name: 'index',
  components: {
    VmProductsList,
    VmHero,
    Promo,
    Categoria
  }
};
</script>
