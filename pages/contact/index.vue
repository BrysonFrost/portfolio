<template>
  <div class="container">
    <h1>Contact Me</h1>
    <h6>Thank you for deciding to contact me, please fill out the form below and I will get back to you as soon as I can
    </h6>
    <form>
      <div class="my-4">
        <div class="row">
          <div class="col-md-6 mb-md-0 mb-3">
            <input type="text" class="form-control" id="nameinput" placeholder="Your Name :">
          </div>
          <div class="col-md-6">
            <input type="email" class="form-control" id="emailinput" placeholder="Email Address :">
          </div>
        </div>

        <div class="mb-3 mt-4">
          <h6 class="">Inquiry Type</h6>
          <input type="radio" class="btn-check" name="inquirytype" id="optionbusiness" autocomplete="off" checked>
          <label class="btn me-2" for="optionbusiness">Business</label>

          <input type="radio" class="btn-check" name="inquirytype" id="optionpersonal" autocomplete="off">
          <label class="btn" for="optionpersonal">Personal</label>
        </div>
        <div class="mb-3">
          <input type="text" class="form-control" id="subjectinput" placeholder="Message Subject :">
        </div>
        <div class="mb-3">
          <textarea class="form-control" id="messageinput" rows="5" placeholder="Your Message :"></textarea>
        </div>
        <button type="submit" class="btn btn-primary">Send Message</button>
      </div>
    </form>
  </div>
</template>