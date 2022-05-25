<template>
  <div class="container">
    <div class="contact-content">
      <div class="contact-header">
        <h2 class="contact-title">Get in touch</h2>
      </div>

      <div class="contact-body">
        <form class="contactform">
          <div class="row g-4">
            <div class="col-lg-6 col-12">
              <div class="inputbox">
                <label for="fullname" class="inputlabel">Enter Full Name</label>
                <input id="fullname" type="text" placeholder="Enter Full Name" class="inputfield">
              </div>
            </div>

            <div class="col-lg-6 col-12">
              <div class="inputbox">
                <label for="emailaddress" class="inputlabel">Enter Email Address</label>
                <input id="emailaddress" type="email" placeholder="Enter Email Address" class="inputfield">
              </div>
            </div>
          </div>

          <div class="row g-4">
            <div class="col-lg-6 col-12">
              <div class="inputbox">
                <label for="phonenumber" class="inputlabel">Enter Phone Number</label>
                <input id="phonenumber" type="tel" pattern="[0-9]{3}-[0-9]{8}" placeholder="Enter Phone Number" class="inputfield">
              </div>
            </div>

            <div class="col-lg-6 col-12">
              <div class="inputbox">
                <label for="subject" class="inputlabel">Enter Subject</label>
                <input id="subject" type="text" placeholder="Enter Subject" class="inputfield">
              </div>
            </div>
          </div>

          <div class="row">
            <div class="col-12">
              <div class="inputbox">
                <label for="message" class="inputlabel">Enter Your Message</label>
                <textarea id="message" class="inputfield" rows="8" placeholder="Enter your message"></textarea>
              </div>
            </div>
          </div>
          
          <div class="formsubmit">
            <button class="btn-submit" type="button">
              <span class="btn-text">Send</span>
            </button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'ContactForm'
  }
</script>