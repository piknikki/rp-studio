<template >
  <div id="work">
    <h3> <i class="fal fa-pencil-paintbrush fa-2x"></i> My Work</h3>
    <div id="card">
      <img class="work-image" src="https://picsum.photos/200" alt="image of artwork">
      <img class="work-image" src="https://picsum.photos/200" alt="image of artwork">
      <img class="work-image" src="https://picsum.photos/200" alt="image of artwork">
      <img class="work-image" src="https://picsum.photos/200" alt="image of artwork">
      <img class="work-image" src="https://picsum.photos/200" alt="image of artwork">
      <img class="work-image" src="https://picsum.photos/200" alt="image of artwork">
      <img class="work-image" src="https://picsum.photos/200" alt="image of artwork">
    </div>
  </div>
</template>

<script>
export default {
  name: 'work',
  data () {
    return {
      art: [
        {
          id: 1,
          loc: '../assets/images/logo.png'
        }
      ]
    }
  }
}
</script>

<style>
#work {
  background-color: white;
  color: #2c3e50;
  padding: 100px;
}

#card {
  display: flex;
  flex-flow: row wrap;
  align-content: center;
  justify-content: space-around;
}

.work-image {
  padding: 20px;
}

</style>
