<template>
  <div class="container">
    <div class="doctordetails-content">
      <div class="row g-4">
        <!-- DOCTOR PROFILE INFO START -->
        <div class="col-lg-4 col-12">
          <div class="profileinfo">
            <!-- DOCTOR PROFILE START -->
            <figure class="doctor-profile">
              <img src="~/static/assets/images/doctors/doctor-7.png" alt="doctor-profile">
            
              <div class="docinfo">
                <h6 class="name">Hasan Al Jahan Rocky</h6>
                <p class="designation">ক্যান্সার, অর্থোসার্জারী ও প্লাষ্টিক সার্জারি বিশেষজ্ঞ</p>
              </div>
            </figure>
            <!-- DOCTOR PROFILE END -->

            <!-- DOCTOR BIOGRAPHY START -->
            <div class="biography">
              <div class="biography-header">
                <h5 class="biography-title">Biography</h5>
              </div>

              <div class="biography-body">
                <p class="biography-text">
                  Physician or scientist, or group, whose work has led to significant advances in the fields of health care and scientific research.
                </p>
              </div>
            </div>
            <!-- DOCTOR BIOGRAPHY END -->
          </div>
        </div>
        <!-- DOCTOR PROFILE INFO END -->
        
        <!-- PROFILE DETAILS START -->
        <div class="col-lg-8 col-12">
          <div class="profile-information">
            <h5 class="name">Hasan Al Jahan Rocky</h5>

            <!-- DOCTOR STUDYLIST START -->
            <ul class="studylist">
              <li class="studylist-item">
                MBBS (Dhaka), BCS (Health)
              </li>
              <li class="studylist-item">
                MS, MCPS (অর্থোসার্জারী)
              </li>
              <li class="studylist-item">
                Diploma In প্লাষ্টিক সার্জারি
              </li>
              <li class="studylist-item">
                Consultant (ক্যান্সার)
              </li>
            </ul>
            <!-- DOCTOR STUDYLIST END -->

            <!-- DOCTOR WORKING PLACE -->
            <p class="workingplace">National Institute of Cancer Research & Hospital (NICRH)</p>
          
            <!-- DOCTOR SPECILITIES START -->
            <div class="specilities">
              <div class="specilities-header">
                <h5 class="specilities-title">Specilities</h5>
              </div>

              <div class="specilities-body">
                <span class="spacility">ক্যান্সার</span>
                <span class="spacility">প্লাষ্টিক সার্জারি</span>
                <span class="spacility">অর্থোসার্জারী</span>
              </div>
            </div>
            <!-- DOCTOR SPECILITIES END -->

            <!-- DOCTOR EXPERIENCE START -->
            <div class="experience">
              <h5 class="experience-title">Experience</h5>
              <p class="experience-text">Surgeon</p>
            </div>
            <!-- DOCTOR EXPERIENCE END -->

            <!-- DOCTOR CONTACT-INFO START -->
            <div class="contacts">
              <div class="contacts-header">
                <h5 class="contacts-title">Share On</h5>
              </div>

              <div class="contacts-body">
                <ul class="followlist">
                  <li class="followlist-item">
                    <VueCustomTooltip label="Share on Facebook">
                      <a href="https://www.facebook.com" target="_blank" class="followlist-link">
                        <i class="fa-brands fa-facebook-f"></i>
                      </a>
                    </VueCustomTooltip>
                  </li>

                  <li class="followlist-item">
                    <VueCustomTooltip label="Share on Twitter">
                      <a href="https://www.twitter.com" target="_blank" class="followlist-link">
                        <i class="fa-brands fa-twitter"></i>
                      </a>
                    </VueCustomTooltip>
                  </li>

                  <li class="followlist-item">
                    <VueCustomTooltip label="Share on Instagram">
                      <a href="https://www.instagram.com" target="_blank" class="followlist-link">
                        <i class="fa-brands fa-instagram"></i>
                      </a>
                    </VueCustomTooltip>
                  </li>

                  <li class="followlist-item">
                    <VueCustomTooltip label="Share on Linkedin">
                      <a href="https://www.linkedin.com" target="_blank" class="followlist-link">
                        <i class="fa-brands fa-linkedin-in"></i>
                      </a>
                    </VueCustomTooltip>
                  </li>
                </ul>
              </div>
            </div>
            <!-- DOCTOR CONTACT-INFO END -->

            <!-- DOCTOR CHEMBER START -->
            <div class="chember">
              <div class="chember-header">
                <h5 class="chember-title">Appointments</h5>
              </div>

              <div class="chember-body">
                <ul class="schedulelist">
                  <li class="schedulelist-item">
                    <span class="daytime">
                      <span class="icon">
                        <i class="fa-regular fa-clock"></i>
                      </span>
                      <span class="text">Thursday (5PM-10PM)</span>  
                    </span>

                    <span class="chambername">
                      <span class="icon">
                        <i class="fa-regular fa-hospital"></i>
                      </span>
                      <span class="text">Abedin Hospital</span>
                    </span>

                    <span class="chamberaddress">
                      <span class="icon">
                        <i class="fa-solid fa-location-dot"></i>
                      </span>
                      <span class="text">Sadar Hospital Road, Narayanpur, Sherpur Town, Sherpur</span>
                    </span>
                    <span class="chember-contact">
                      <span class="icon">
                        <i class="fa-solid fa-phone"></i>
                      </span>
                      <a href="tel:+8801615922742" class="link">+8801615922742</a>
                    </span>
                    <!-- <button class="btn-appointment" type="button">Appointment</button> -->
                  </li>
                  
                  <li class="schedulelist-item">
                    <span class="daytime">
                      <span class="icon">
                        <i class="fa-regular fa-clock"></i>
                      </span>
                      <span class="text">Thursday (5PM-10PM)</span>  
                    </span>

                    <span class="chambername">
                      <span class="icon">
                        <i class="fa-regular fa-hospital"></i>
                      </span>
                      <span class="text">Abedin Hospital</span>
                    </span>

                    <span class="chamberaddress">
                      <span class="icon">
                        <i class="fa-solid fa-location-dot"></i>
                      </span>
                      <span class="text">Sadar Hospital Road, Narayanpur, Sherpur Town, Sherpur</span>
                    </span>
                    <span class="chember-contact">
                      <span class="icon">
                        <i class="fa-solid fa-phone"></i>
                      </span>
                      <a href="tel:+8801615922742" class="link">+8801615922742</a>
                    </span>
                    <!-- <button class="btn-appointment" type="button">Appointment</button> -->
                  </li>
                </ul>
              </div>
            </div>
            <!-- DOCTOR CHEMBER END -->
          </div>
        </div>
        <!-- PROFILE DETAILS END -->
      </div>
    </div>
  </div>
</template>

<script>
  import VueCustomTooltip from '@adamdehaven/vue-custom-tooltip';
  export default {
    name: 'DoctorDetails',
    components: {
      VueCustomTooltip
    }
  }
</script>