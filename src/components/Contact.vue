<template>
  <div>
    <h3> <i class="fal fa-cat-space fa-2x"></i> Contact me</h3>
    <br>
    <div id="contact">
      <form id="form" name="contact" method="POST" data-netlify="true">
        <p>
          <label>Your Name: <input type="text" name="name" /></label>
        </p>
        <p>
          <label>Your Email: <input type="email" name="email" /></label>
        </p>
        <p>
          <label>Message: <textarea name="message"></textarea></label>
        </p>
        <p>
          <button type="submit">Send</button>
        </p>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'contact'
}
</script>

<style scoped>
#contact {
  display: flex;
  justify-content: center;
}
#form {
  width: 300px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
  font-size: 1.5em;
}

input, textarea {
  padding: 10px;
  border-radius: 5px;
}

</style>
