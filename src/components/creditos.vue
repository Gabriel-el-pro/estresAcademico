<template>
    <div>
        <v-container>
            
<div class="v-dialog v-dialog--active" style="max-width: 480px; margin-top:-10px">
<div class="v-card v-sheet theme--light">
<div class="v-card__title  primary green accent-2 v-card__title--primary">
<h2 class="text-uppercase headline">Desarrollador del producto.</h2>
</div>
<div class="v-card__text ">
<div role="list" class="v-list transparent theme--light">
<div role="listitem">
<div class="v-list__tile v-list__tile--avatar theme--light">
<div class="v-list__tile__content">
<div class="v-list__tile__title font-weight-bold">Juan Gabriel Salgado Bolaño.</div>
</div>
<div class="v-list__tile__avatar">
    <div class="v-avatar" style="height: 70px; width: 70px;">
    <img src="../../public/yo.jpeg" @click="verArdwin()">
 </div>
 <v-dialog
            v-model="persona"
            :overlay="false"
            max-width="400px"
            transition="dialog-transition"
            
          >
            <v-card :img="info.avatar" width="400" height="500" class="buelta" >
              
            </v-card>
          </v-dialog>
    </div>
     </div>
           </div>

    
<div role="listitem">
<div class="v-list__tile v-list__tile--avatar theme--light">
 <div class="v-list__tile__content">
 
</div>

     </div>
     </div>
     <hr class="v-divider theme--light">
     <div role="listitem" class="primary pink accent-2 mt-4">
     <div class="v-list__tile theme--light">
<div class="v-list__tile__avatar">
 
  <v-dialog
  v-model="persona"
  :overlay="false"
  max-width="400px"
  transition="dialog-transition"
>
  <v-card :img="info.avatar" width="400" height="500">
    
  </v-card>
</v-dialog>
       </div>
       </div>
       </div>
 <div class="v-list__tile__content"> 
<img src="../../public/unicor.png" class="ml-4 mt-4" width="200px" height="80px">

<h2 class="text-uppercase red">Referencias</h2>
<p class="text-uppercase blue" style="font-weight: bold;">Móatani, A. [@aventuramoatani4773]. (2019, abril 30). Estrés academico. Youtube. https://www.youtube.com/watch?v=Aydb_cWXbjc
  Zambrano, D. [@rositaybruce]. (2019, mayo 5). ¿Qué es el estrés académico? Youtube. https://www.youtube.com/watch?v=nOSkHi8O8OY</p>


                </div>
                </div>
                </div>
                </div>
                </div>
        </v-container>
    </div>
</template>
<script>
export default {
    name:"App",
    data: () =>{
       return {
      info: {},
      dialog: false,
      persona: false
    }
    },
    methods: {

    verArdwin () {
      this.info = {
        nombre: 'Gabriel Salgado',
        avatar: require('../../public/yo.jpeg')
      }
      this.persona = true
    },
  },
}
</script>
<style scoped>
@media (max-width: 500px) {
  .buelta{
   transform: rotate(90deg);
  }
}
</style>
 




