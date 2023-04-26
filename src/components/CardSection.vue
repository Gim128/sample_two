<template>
  <div class="text-summery">
    <h1>SUMMERY OF US</h1>
  </div>

  <div id="cards-section">
    <div class="card">
      <div class="image-container">
        <img
          src="https://images.unsplash.com/photo-1612814251241-6089fc8fee42?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=327&q=80"
          alt=""
        />
      </div>
      <div class="text-container">
        <span class="title">New Horizons</span>
        <h5>Neil Rosenstesch</h5>
        <span>- Banff, Canada.</span>
        <p>
          Lorem ipsum dolor sit amet, consec tetur adipiscing elit. Vivamus a porta
          turpis. Nunc vitae diam non tellus tincidunt dictum eu ut tellus.
        </p>
      </div>
    </div>
    <div class="card">
      <!--Change class="card"-->
      <div class="image-container">
        <img
          src="https://images.unsplash.com/photo-1653760654335-9d9b0f6357f0?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=327&q=80"
          alt=""
        />
      </div>
      <div class="text-container">
        <span class="title">New Roads</span>
        <h5>Neil Rosenstesch</h5>
        <span>- Banff, Canada.</span>
        <p>
          Lorem ipsum dolor sit amet, consec tetur adipiscing elit. Vivamus a porta
          turpis. Nunc vitae diam non tellus tincidunt dictum eu ut tellus.
        </p>
      </div>
    </div>
    <div class="card">
      <!--Change class="card"-->
      <div class="image-container">
        <img
          src="https://images.unsplash.com/photo-1678625741301-a5a38243ed01?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=327&q=80"
          alt=""
        />
      </div>
      <div class="text-container">
        <span class="title">New Roads</span>
        <h5>Neil Rosenstesch</h5>
        <span>- Banff, Canada.</span>
        <p>
          Lorem ipsum dolor sit amet, consec tetur adipiscing elit. Vivamus a porta
          turpis. Nunc vitae diam non tellus tincidunt dictum eu ut tellus.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    $(".hover-complete").mouseleave(function () {
      $(this).removeClass("hover-complete");
      $(this).addClass("card");
    });
  },
};
</script>

<style scoped>
.text-summery {
  text-align: center;
  font-size: large;
  margin-top: 114px;
  font-size: 36px;
  transition: width 2s;
}

#cards-section {
  padding: 6% 0px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0;
  -webkit-user-select: none;
  -moz-user-select: none;
  user-select: none;
}
#cards-section .card {
  background: transparent;
  border-radius: 7px;
  text-align: center;
  position: relative;
  display: inline-block;
  overflow: hidden;
  margin: 0px 18px;
  min-width: 220px;
  max-width: 320px;
  width: 100%;
  box-shadow: 0px 5px 15px 0px rgba(0, 0, 0, 0.3), -5px 5px 15px 0px rgba(0, 0, 0, 0.3);
}
#cards-section .card .image-container img {
  -webkit-transition: all 0.4s ease-in;
  -moz-transition: all 0.4s ease-in;
  -o-transition: all 0.4s ease-in;
  -ms-transition: all 0.4s ease-in;
  transition: all 0.4s ease-in;
  z-index: 1;
  position: relative;
  vertical-align: top;
  max-width: 100%;
}
#cards-section .card:hover .image-container img {
  -webkit-transform: scale(1.15);
  -moz-transform: scale(1.15);
  -ms-transform: scale(1.15);
  -o-transform: scale(1.15);
  transform: scale(1.15);
}
#cards-section .card .image-container i {
  -webkit-transition: all 0.4s ease-in;
  -moz-transition: all 0.4s ease-in;
  -o-transition: all 0.4s ease-in;
  -ms-transition: all 0.4s ease-in;
  transition: all 0.4s ease-in;
  position: absolute;
  color: #ffffff;
  z-index: 99;
  margin: 18px 0 0 285px;
  opacity: 0;
}
#cards-section .card:hover .image-container i {
  opacity: 1;
}
#cards-section .card .text-container {
  -webkit-transition: all 0.4s ease-in;
  -moz-transition: all 0.4s ease-in;
  -o-transition: all 0.4s ease-in;
  -ms-transition: all 0.4s ease-in;
  transition: all 0.4s ease-in;
  opacity: 1;
  z-index: 10;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  margin: 110% 0 0 0;
  padding: 8%;
  text-align: left;
  vertical-align: bottom;
  color: #ffffff;
}
#cards-section .card:hover .text-container {
  margin: 85% 0 0 0;
}
#cards-section .card .text-container span.title {
  font-family: "Raleway", sans-serif;
  font-size: 16px;
  letter-spacing: 1px;
  margin: 0px;
  font-weight: 400;
}
#cards-section .card .text-container h5 {
  font-family: "Roboto", sans-serif;
  font-size: 23px;
  letter-spacing: 1px;
  margin: 8px 0px 0px 0px;
  font-weight: 700;
}
#cards-section .card .text-container span {
  font-family: "Raleway", sans-serif;
  font-size: 13px;
  letter-spacing: 1px;
  margin-top: 1px;
  text-transform: uppercase;
  font-weight: 700;
}
#cards-section .card .text-container p {
  -webkit-transition: all 0.4s ease-in;
  -moz-transition: all 0.4s ease-in;
  -o-transition: all 0.4s ease-in;
  -ms-transition: all 0.4s ease-in;
  transition: all 0.4s ease-in;
  font-family: "Raleway", sans-serif;
  font-size: 13px;
  letter-spacing: 1px;
  margin-top: 10px;
  line-height: 20px;
  opacity: 0;
}
#cards-section .card:hover .text-container p {
  opacity: 1;
}
/*----------MEDIA QUERIES RESPONSIVE----------*/
@media (min-width: 320px) and (max-width: 479px) {
  #cards-section {
    display: grid;
    align-items: center;
    justify-content: center;
  }
  #cards-section .card {
    margin: 10px 0px;
  }
  #cards-section .card:hover .text-container {
    margin: 82% 0 0 0;
  }
  #cards-section .card .image-container i {
    margin: 18px 0 0 270px;
  }
}
@media (min-width: 480px) and (max-width: 599px) {
  #cards-section {
    display: grid;
    align-items: center;
    justify-content: center;
  }
  #cards-section .card {
    margin: 10px 0px;
  }
}
@media (min-width: 600px) and (max-width: 767px) {
  #cards-section .card:hover .text-container {
    margin: 65% 0 0 0;
  }
  #cards-section .card .image-container i {
    margin: 18px 0 0 230px;
  }
}
/*########  YOU DONT  #########
  #########  NEED THIS  #########
  ######  ONLY FOR DEMO  #####*/
#cards-section .hover-complete {
  background: transparent;
  border-radius: 7px;
  text-align: center;
  position: relative;
  display: inline-block;
  overflow: hidden;
  margin: 0px 18px;
  min-width: 220px;
  max-width: 320px;
  width: 100%;
  box-shadow: 0px 5px 15px 0px rgba(0, 0, 0, 0.3), -5px 5px 15px 0px rgba(0, 0, 0, 0.3);
}
#cards-section .hover-complete .image-container img {
  z-index: 1;
  position: relative;
  vertical-align: top;
  max-width: 100%;
  -webkit-transform: scale(1.15);
  -moz-transform: scale(1.15);
  -ms-transform: scale(1.15);
  -o-transform: scale(1.15);
  transform: scale(1.15);
}
#cards-section .hover-complete .image-container i {
  position: absolute;
  color: #ffffff;
  z-index: 99;
  margin: 18px 0 0 285px;
  opacity: 1;
}
#cards-section .hover-complete .text-container {
  opacity: 1;
  z-index: 10;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  margin: 85% 0 0 0;
  padding: 8%;
  text-align: left;
  vertical-align: bottom;
  color: #ffffff;
}
#cards-section .hover-complete .text-container span.title {
  font-family: "Raleway", sans-serif;
  font-size: 16px;
  letter-spacing: 1px;
  margin: 0px;
  font-weight: 400;
}
#cards-section .hover-complete .text-container h5 {
  font-family: "Roboto", sans-serif;
  font-size: 23px;
  letter-spacing: 1px;
  margin: 8px 0px 0px 0px;
  font-weight: 700;
}
#cards-section .hover-complete .text-container span {
  font-family: "Raleway", sans-serif;
  font-size: 13px;
  letter-spacing: 1px;
  margin-top: 1px;
  text-transform: uppercase;
  font-weight: 700;
}
#cards-section .hover-complete .text-container p {
  -webkit-transition: all 0.4s ease-in;
  -moz-transition: all 0.4s ease-in;
  -o-transition: all 0.4s ease-in;
  -ms-transition: all 0.4s ease-in;
  transition: all 0.4s ease-in;
  font-family: "Raleway", sans-serif;
  font-size: 13px;
  letter-spacing: 1px;
  margin-top: 10px;
  line-height: 20px;
  opacity: 1;
}
@media (min-width: 320px) and (max-width: 479px) {
  #cards-section {
    display: grid;
    align-items: center;
    justify-content: center;
  }
  #cards-section .hover-complete {
    margin: 10px 0px;
  }
  #cards-section .hover-complete .text-container {
    margin: 82% 0 0 0;
  }
  #cards-section .hover-complete .image-container i {
    margin: 18px 0 0 270px;
  }
}
@media (min-width: 480px) and (max-width: 599px) {
  #cards-section {
    display: grid;
    align-items: center;
    justify-content: center;
  }
  #cards-section .hover-complete {
    margin: 10px 0px;
  }
}
@media (min-width: 600px) and (max-width: 767px) {
  #cards-section .hover-complete .text-container {
    margin: 65% 0 0 0;
  }
  #cards-section .hover-complete .image-container i {
    margin: 18px 0 0 230px;
    opacity: 1;
  }
}
</style>
