<template>
<div>
  <v-card color="grey lighten-2">
    <v-img :src="dog.img" height="170px"></v-img>
    <v-card-title>
      <div>
        <h3>{{dog.name}}</h3>
        <p>{{dog.breed}}</p>
      </div>
    </v-card-title>
  </v-card>
  <v-btn @click="$emit('addToFavorites', dog)">Add to Favorites</v-btn>
</div>
</template>

<script>
export default {
  props: {
	    dog: {
	      type: Object
	    }
	  }
};
</script>
