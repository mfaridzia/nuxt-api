<template>
  <div class="container">
     <ul class="menu">
      <li> <router-link to="/"> Home </router-link> </li>
      <li> <router-link to="/about"> About </router-link> </li>
      <li> <router-link to="/contact"> Contact </router-link> </li>
    </ul>
     <section class="content">
         <p>
             Hello my name is YOUR NAME Lorem ipsum dolor sit amet, consectetur adipisicing elit. Soluta, a debitis omnis 
             nam obcaecati eius minima excepturi sint ab asperiores? Nam dolorum voluptas ad quaerat 
             suscipit voluptates perferendis, pariatur sed!
         </p>
     </section>
  </div>
</template>

<style scoped>
.container {
  width: 75%;
  margin: 100px auto;
  text-align: center;
}
.content p {
    text-align: justify;
}
.menu {
   list-style: none;
   margin-bottom: 20px;
}
.menu li {
  display: inline;
}
.menu li a {
  padding: 20px;
  text-decoration: none;
}
</style>
