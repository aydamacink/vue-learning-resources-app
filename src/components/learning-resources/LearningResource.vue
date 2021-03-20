<template>
  <li>
    <div>
      <header>
        <h3>{{title}}</h3>
        <button>Delete</button>
      </header>
    </div>
    <p>{{description}}</p>
    <nav>
      <a :href="link">View Resource</a> 
      <!-- QUESTION: why does the link have to be bound with : , different from the other props?  -->
    </nav>
  </li>
</template>

<script>
export default {
  props:['title', 'description', 'link']
}
</script>