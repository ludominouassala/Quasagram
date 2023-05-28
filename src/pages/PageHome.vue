<template>
  <q-page class="constrain q-pa-md">

    <div class="row q-col-gutter-lg">
      <div class="col-12 col-sm-8">
        <q-card
          v-for="post in posts" 
          :key="post.id" 
          class="card-post q-mb-md" 
          flat bordered>
      <q-item>
        <q-item-section avatar>
          <q-avatar size="50px">
            <img src="~src/pages/favicon-32x32.png">
          </q-avatar>
        </q-item-section>

        <q-item-section>
          <q-item-label class="text-bold">Ludo_Uassala</q-item-label>
          <q-item-label caption>
            {{ post.location }}
          </q-item-label>
        </q-item-section>
      </q-item>

      <q-separator />

      <q-img src="~src/pages/down.jpg"/>

      <q-card-section>
        <div>I Can Be All I Want</div>
        <div class="text-caption text-grey">May 23 At 01:50AM</div>
      </q-card-section>
    </q-card>

      </div>
      <div class="col-3 large-screen-only">
         <q-item class="fixed">
        <q-item-section avatar>
          <q-avatar size="58px">
            <img src="~src/pages/favicon-32x32.png">
          </q-avatar>
        </q-item-section>

        <q-item-section>
          <q-item-label class="text-bold">Ludo_Uassala</q-item-label>
          <q-item-label caption>
            Ludo_Uassala
          </q-item-label>
        </q-item-section>
      </q-item>

      </div>
    </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageHome',
  data() {
    return{
      posts: [
      {
      id: 1,
      caption: 'Be What you Want To Be',
      location: 'Maputo,Mozambique',
      image: '~src/pages/down.jpg'
       },
       {
      id: 1,
      caption: 'Be What you Want To Be',
      location: 'Maputo,Mozambique',
      image: '~src/pages/down.jpg'
       },
       {
      id: 1,
      caption: 'Be What you Want To Be',
      location: 'Maputo,Mozambique',
      image: '~src/pages/down.jpg'
       }
      ]
    }
  }
}
</script>

<style lang="sass">
  .card-post
   .q-img
    min-height:370px
</style>
