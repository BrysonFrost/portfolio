<script setup>
const model = defineModel()

</script>
<template>
  <div class="container col-lg-8 col-xl-7 mt-5">
    <div class="text-center">
      <h1>Contact Me</h1>
      <h6>Thank you for deciding to contact me. Please fill out the form below and I will get back to you at the entered
        email address as soon as I can</h6>
    </div>

    <form>
      <div class="my-4">
        <div class="row">
          <div class="col-12 col-xl-5">
            <div class="row">
              <div class="mb-4 col-xl-12 col-md-6">
                <input type="text" name="name" v-model="name" class="form-control" placeholder="Your Name :">
              </div>
              <div class="mb-4 col-xl-12 col-md-6">
                <input type="email" name="email" v-model="email" class="form-control" placeholder="Email Address :">
              </div>
            </div>

            <div class="mb-4">
              <input type="text" name="subject" v-model="subject" class="form-control" placeholder="Message Subject :">
            </div>
          </div>

          <div class="mb-4 col-xl-7">
            <textarea class="form-control" name="message" v-model="message" rows="6" placeholder="Your Message :"></textarea>
          </div>
        </div>

        <div class="d-flex flex-row-reverse">
          <button type="submit" class="btn btn-primary">Send Message</button>
        </div>

      </div>
    </form>

  </div>

</template>