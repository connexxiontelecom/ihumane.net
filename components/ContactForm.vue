<template>
  <div class="contact-form-section section-padding-t90-b100" :style="{backgroundColor: '#f8faff'}">
    <div class="container">
      <div class="row">
        <div class="offset-lg-2 col-lg-8">
          <!-- Section Title Start -->
          <div class="section-title text-center" data-aos="fade-up">
            <h2 class="title fz-32">Make Enquiries</h2>
            <p class="sub-title">Are you beaming with questions or unclear on certain areas of iHumane you’d like to
              address? Please reach out to us lets talk…</p>
          </div>
          <!-- Section Title End -->
          <div class="contact-form">
            <form>
              <div class="row mtn-30">
                <div class="col-md-6 col-12 mt-30">
                  <input type="text" placeholder="Your Name *" name="name">
                </div>
                <div class="col-md-6 col-12 mt-30">
                  <input type="email" placeholder="Email *" name="email">
                </div>
                <div class="col-md-12 col-12 mt-30">
                  <input type="text" placeholder="Subject *" name="subject">
                </div>
                <div class="col-12 mt-30">
                  <textarea name="message" placeholder="Message"></textarea>
                </div>
                <div class="col-12 text-center mt-30">
                  <button class="btn btn-primary btn-hover-secondary">Submit</button>
                </div>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
