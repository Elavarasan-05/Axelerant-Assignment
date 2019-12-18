<template>
  <div class="contact-container" :style="{ background: 'url(' + backgroundImage + ')' }">
    <div class="conatct-form-container">
      <h2>Convinced To Work With Us?</h2>
      <p>Company has helped agencies keep their promises to client since 2005</p>
      <form>
      <div class="contact-form">
        <div class="input-filed">
          <input type="text" placeholder="Fullname">
        </div>
        <div class="input-filed">
          <input type="email" placeholder="Email Address">
        </div>
        <div class="input-filed">
          <input type="number" placeholder="Phone Number">
        </div>
      </div>
      <div class="message-desc">
        <textarea placeholder="Message in berif"></textarea>
      </div>
      <div class="form-submit">
        <button type="submit">Submit</button>
      </div>
      </form>
    </div>
  </div>
</template>
<script>
export default {
  data(){
    return {
      backgroundImage: require('../assets/contact.png')
    }
  }
}
</script>

