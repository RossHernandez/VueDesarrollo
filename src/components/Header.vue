<template>
   <div>
        <nav class="nabvar-principal" role="navigation">
            <div class="nav-wrapper container">
            <ul class="right">
                <li>
                <a href="#" class="mt10">
                  
                </a>
            </li>
            </ul>
            <ul id="nav-mobile" class="sidenav background-menu">
                <div class="mt40"></div>
                <div class="divider"></div>
                <li ><a href="#"><i class="material-icons color-icon">settings</i>Ajustes</a></li>
                <div class="divider"></div>
                <li ><a href="#"><i class="material-icons color-icon">email</i>Contacto</a></li>
                <div class="divider"></div>
                <li ><a href="#"><i class="material-icons color-icon">account_balance_wallet</i>Formas pago</a></li>
                <div class="divider"></div>
                <li ><a href="#"><i class="material-icons color-icon">perm_phone_msg</i>Teléfono</a></li>
                <div class="divider"></div>
                <li ><a href="#"><i class="material-icons color-icon">assignment</i>Legales</a></li>
            </ul>
            <a href="#" data-target="nav-mobile" class="sidenav-trigger"><i class="material-icons color-icon">menu</i></a>
            </div>
        </nav>
   </div>
</template>
<script>

export default {
  name: 'Header',
  components: {
    
  }
}
</script>
<style>

/* Menu Principal */
.color-icon {
  color:#E96811 !important;
}
.background-menu{
  background-color:  #242021 ;
  border-left: 40px solid #E96811;

}
.sidenav li > a {
  color:#FFFFFF !important;
  font-size: 17px;
}
.sidenav > .divider{
  background-color: #707070 !important;
}
.nabvar-principal{
  background-color: #FFFFFF;
}
</style>