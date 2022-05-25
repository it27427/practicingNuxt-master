<template>
  <div class="container">
    <div class="doctordetails-content">
      <div class="row g-4">
        <div class="col-lg-3 col-12">
          <figure class="doctor-profile">
            <img src="~/static/assets/images/doctors/doctor-7.png" alt="doctor-profile">
          </figure>
        </div>
        
        <div class="col-lg-9 col-12">
          <div class="profile-information">
            <h6 class="name">Hasan Al Jahan Rocky</h6>
            <p class="speciality">ক্যান্সার, অর্থোসার্জারী ও প্লাষ্টিক সার্জারি বিশেষজ্ঞ</p>
            <p class="degree">MBBS, Mymensingh Medical College</p>
          </div>
        </div>
      </div>

      <div class="row">
        <div class="col-12">
          <div class="doctor-summary">
            <p class="doctortext">
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sit repellendus neque tempore esse minus sed.
            </p>
            <p class="area">Treatment area</p>
          </div>
        </div>
      </div>

      <div class="row">
        <div class="col-12">
          <ul class="schedulelist">
            <li class="sehedulelist-item">
              <span class="chamber-info">
                <span class="chambername">Chamber name</span>
                <span class="chamberaddress">Chamber address</span>
                <span class="daytime">Appointment day and time</span>
              </span>

              <button class="btn-appointment" type="button">Appointment</button>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'DoctorDetails'
  }
</script>