<template>
    <div class="container bootdey">
        <div class="row">
            <div class="col-12 text-center skills">
                <div class="section-title my-5">
                    <h4 id="skills" class="title mb-4 text-uppercase fw-bold ">Skills</h4>
                </div>
            </div><!--end col-->
        </div><!--end row-->

        <div class="row">
            <div class="col-lg-3 col-md-6 col-12 mt-4 pt-2">
                <div class="team text-center rounded py-4">
                    <img :src="require('@/assets/img/html.png')" class="img-fluid avatar avatar-medium shadow rounded-pill" alt="">
                    <div class="content mt-3">
                        <h4 class="title mb-0"><strong>HTML5</strong></h4>
                    </div>
                </div>
            </div><!--end col-->
            
            <div class="col-lg-3 col-md-6 col-12 mt-4 pt-2">
                <div class="team text-center rounded py-4">
                    <img :src="require('@/assets/img/css.png')" class="img-fluid avatar avatar-medium shadow rounded-pill" alt="">
                    <div class="content mt-3">
                        <h4 class="title mb-0"><strong>CSS3</strong></h4>
                    </div>
                </div>
            </div><!--end col-->
            
            <div class="col-lg-3 col-md-6 col-12 mt-4 pt-2">
                <div class="team text-center rounded py-4">
                    <img :src="require('@/assets/img/php.png')" class="img-fluid avatar avatar-medium shadow rounded-pill" alt="">
                    <div class="content mt-3">
                        <h4 class="title mb-0"><strong>PHP</strong></h4>
                    </div>
                </div>
            </div><!--end col-->
            
            <div class="col-lg-3 col-md-6 col-12 mt-4 pt-2">
                <div class="team text-center rounded py-4">
                    <img :src="require('@/assets/img/js.png')" class="img-fluid avatar avatar-medium shadow rounded-pill" alt="">
                    <div class="content mt-3">
                        <h4 class="title mb-0"><strong>Javascript</strong></h4>
                    </div>
                </div>
            </div><!--end col-->
        </div><!--end row-->
    </div>
</template>

<style>
body{margin-top:20px;}

.skills{
  letter-spacing: 18px;
}
.team-list img {
  width: 50%;
}

.team-list .content {
  width: 50%;
}

.team-list .content .follow {
  position: absolute;
  bottom: 24px;
}

.team-list:hover {
  -webkit-transform: scale(1.05);
          transform: scale(1.05);
}

.team, .team-list {
  -webkit-transition: all 0.5s cubic-bezier(0.68, -0.55, 0.27, 1.55) 0s;
  transition: all 0.5s cubic-bezier(0.68, -0.55, 0.27, 1.55) 0s;
}

.team .content .title, .team-list .content .title {
  font-size: 18px;
}

.team .overlay {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  opacity: 0;
  -webkit-transition: all 0.5s ease;
  transition: all 0.5s ease;
}

.team .member-position, .team .team-social {
  position: absolute;
  bottom: -35px;
  right: 0;
  left: 0;
  margin: auto 10%;
  z-index: 99;
}

.team .team-social {
  bottom: 40px;
  opacity: 0;
  -webkit-transition: all 0.5s cubic-bezier(0.68, -0.55, 0.27, 1.55) 0s;
  transition: all 0.5s cubic-bezier(0.68, -0.55, 0.27, 1.55) 0s;
}

.team:hover {
  -webkit-transform: translateY(-7px);
          transform: translateY(-7px);
  -webkit-box-shadow: 0 0 5px rgba(0, 0, 0, 0.15);
          box-shadow: 0 0 5px rgba(0, 0, 0, 0.15);
}

.team:hover .overlay {
  opacity: 0.6;
}

.team:hover .team-social {
  opacity: 1;
}

@media (max-width: 768px) {
  .team-list img,
  .team-list .content {
    width: 100%;
    float: none !important;
  }
  .team-list img .follow,
  .team-list .content .follow {
    position: relative;
    bottom: 0;
  }
}

.social-icon.social li a {
    color: #adb5bd;
    border-color: #adb5bd;
}
.social-icon li a {
    color: #35404e;
    border: 1px solid #35404e;
    display: inline-block;
    height: 32px;
    text-align: center;
    font-size: 15px;
    width: 32px;
    line-height: 30px;
    -webkit-transition: all 0.4s ease;
    transition: all 0.4s ease;
    overflow: hidden;
    position: relative;
}
.rounded {
    border-radius: 5px !important;
}

.para-desc {
    max-width: 600px;
}
.text-muted {
    color: #8492a6 !important;
}

.section-title .title {
    letter-spacing: 0.5px;
    font-size: 30px;
}
</style>