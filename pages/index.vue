<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest tech news</h1>
    </section>
    <section class="featured-posts">
      <postPreview 
      id="1"
      thumbnail="https://www.google.co.uk/url?sa=i&source=images&cd=&cad=rja&uact=8&ved=2ahUKEwjyvqTbt8feAhVMXhoKHfUOA0wQjRx6BAgBEAU&url=https%3A%2F%2Fwww.bbc.co.uk%2Fprogrammes%2Fp06hpg70&psig=AOvVaw1_0W7EnD8ylFtYTDdE6ktJ&ust=1541857168092313"
      title="Tech"
      previewText="This is preview "
      />
    </section>
  </div>
</template>

<script>
import postPreview from '~/components/Posts/PostPreview'

export default {
  components: {
    postPreview : postPreview
  }
}
</script>

<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

</style>

