<template>
  <div class="card h-100">
    <div class="embed-responsive embed-responsive-16by9">
      <img class="card-img-top embed-responsive-item" :src="'../../'+ category.imageUrl.substring(category.baseURL)"  alt="Category Image">
    </div>
    <!-- :src="'../../' + category.imageUrl"-->
    <div class="card-body">
      <h5 class="card-title">{{category.categoryName}}</h5>
      <p class="card-text font-italic">{{category.description.substring(0,65)}}...</p>
      <router-link id="edit-category" :to="{ name: 'EditCategory', params: { id : category.id, category: category } }" >
        Edit
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
    name : "CategoryBox",
    props : ["category"],
    methods : {
        
    }
}
</script> 

