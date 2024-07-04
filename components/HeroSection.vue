<template>
  <link rel='stylesheet' href='https://cdn.jsdelivr.net/npm/bootstrap@4.4.1/dist/css/bootstrap.min.css'>
  <section class="hero">
   <div class="container">
    <div class="main-body">
    
          <div class="row gutters-sm">
            <div class="col-md-4 mb-3">
              <div class="card">
                <div class="card-body">
                  <div class="d-flex flex-column align-items-center text-center">
                    <img src="data:image/jpeg;base64,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" alt="Admin" class="rounded-circle" width="150">
                    <div class="mt-3">
                      <h4>it's your boy</h4>
                      <p class="text-secondary mb-1">Mahasiswa Amikom</p>
                      <p class="text-muted font-size-sm">YKC condong catur</p>
                      <button class="btn btn-primary">Follow</button>
                      <button class="btn btn-outline-primary">Message</button>
                    </div>
                  </div>
                </div>
              </div>
              <div class="card mt-3">
                <ul class="list-group list-group-flush">
                  <li class="list-group-item d-flex justify-content-between align-items-center flex-wrap">
                    <h6 class="mb-0"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-globe mr-2 icon-inline"><circle cx="12" cy="12" r="10"></circle><line x1="2" y1="12" x2="22" y2="12"></line><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"></path></svg>Website</h6>
                    <span class="text-secondary">https://bootdey.com</span>
                  </li>
                  <li class="list-group-item d-flex justify-content-between align-items-center flex-wrap">
                    <h6 class="mb-0"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-github mr-2 icon-inline"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg>Github</h6>
                    <span class="text-secondary">Alfvonly</span>
                  </li>
                  <li class="list-group-item d-flex justify-content-between align-items-center flex-wrap">
                    <h6 class="mb-0"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-twitter mr-2 icon-inline text-info"><path d="M23 3a10.9 10.9 0 0 1-3.14 1.53 4.48 4.48 0 0 0-7.86 3v1A10.66 10.66 0 0 1 3 4s-4 9 5 13a11.64 11.64 0 0 1-7 2c9 5 20 0 20-11.5a4.5 4.5 0 0 0-.08-.83A7.72 7.72 0 0 0 23 3z"></path></svg>Twitter</h6>
                    <span class="text-secondary">@alfinmuhamd</span>
                  </li>
                  <li class="list-group-item d-flex justify-content-between align-items-center flex-wrap">
                    <h6 class="mb-0"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-instagram mr-2 icon-inline text-danger"><rect x="2" y="2" width="20" height="20" rx="5" ry="5"></rect><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"></line></svg>Instagram</h6>
                    <span class="text-secondary">@alfinmuhamd</span>
                  </li>
                  <li class="list-group-item d-flex justify-content-between align-items-center flex-wrap">
                    <h6 class="mb-0"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-facebook mr-2 icon-inline text-primary"><path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"></path></svg>Facebook</h6>
                    <span class="text-secondary">muhamad alfin</span>
                  </li>
                </ul>
              </div>
            </div>
            <div class="col-md-8">
              <div class="card mb-3">
                <div class="card-body">
                  <div class="row">
                    <div class="col-sm-3">
                      <h6 class="mb-0">Full Name</h6>
                    </div>
                    <div class="col-sm-9 text-secondary">
                      Andi Muahamad Barik Alfin
                    </div>
                  </div>
                  <hr>
                  <div class="row">
                    <div class="col-sm-3">
                      <h6 class="mb-0">Email</h6>
                    </div>
                    <div class="col-sm-9 text-secondary">
                      andimuh27@gmail.com
                    </div>
                  </div>
                  <hr>
                  <div class="row">
                    <div class="col-sm-3">
                      <h6 class="mb-0">Phone</h6>
                    </div>
                    <div class="col-sm-9 text-secondary">
                      (239) 816-9029
                    </div>
                  </div>
                  <hr>
                  <div class="row">
                    <div class="col-sm-3">
                      <h6 class="mb-0">Mobile</h6>
                    </div>
                    <div class="col-sm-9 text-secondary">
                      (320) 380-4539
                    </div>
                  </div>
                  <hr>
                  <div class="row">
                    <div class="col-sm-3">
                      <h6 class="mb-0">Address</h6>
                    </div>
                    <div class="col-sm-9 text-secondary">
                      YKC , depok condong catur
                    </div>
                  </div>
                  <hr>
                  <div class="row">
                  </div>
                </div>
              </div>

              <div class="row gutters-sm">
                <div class="col-sm-6 mb-3">
                  <div class="card h-100">
                    <div class="card-body">
                      <h6 class="d-flex align-items-center mb-3">Project Status</h6>
                      <small>Web Design</small>
                      <div class="progress mb-3" style="height: 5px">
                        <div class="progress-bar bg-primary" role="progressbar" style="width: 80%" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100"></div>
                      </div>
                      <small>Website Markup</small>
                      <div class="progress mb-3" style="height: 5px">
                        <div class="progress-bar bg-primary" role="progressbar" style="width: 72%" aria-valuenow="72" aria-valuemin="0" aria-valuemax="100"></div>
                      </div>
                      <small>One Page</small>
                      <div class="progress mb-3" style="height: 5px">
                        <div class="progress-bar bg-primary" role="progressbar" style="width: 89%" aria-valuenow="89" aria-valuemin="0" aria-valuemax="100"></div>
                      </div>
                      <small>Mobile Template</small>
                      <div class="progress mb-3" style="height: 5px">
                        <div class="progress-bar bg-primary" role="progressbar" style="width: 55%" aria-valuenow="55" aria-valuemin="0" aria-valuemax="100"></div>
                      </div>
                      <small>Backend API</small>
                      <div class="progress mb-3" style="height: 5px">
                        <div class="progress-bar bg-primary" role="progressbar" style="width: 66%" aria-valuenow="66" aria-valuemin="0" aria-valuemax="100"></div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-sm-6 mb-3">
                  <div class="card h-100">
                    <div class="card-body">
                      <h6 class="d-flex align-items-center mb-3">Project Status</h6>
                      <small>Web Design</small>
                      <div class="progress mb-3" style="height: 5px">
                        <div class="progress-bar bg-primary" role="progressbar" style="width: 80%" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100"></div>
                      </div>
                      <small>Website Markup</small>
                      <div class="progress mb-3" style="height: 5px">
                        <div class="progress-bar bg-primary" role="progressbar" style="width: 72%" aria-valuenow="72" aria-valuemin="0" aria-valuemax="100"></div>
                      </div>
                      <small>One Page</small>
                      <div class="progress mb-3" style="height: 5px">
                        <div class="progress-bar bg-primary" role="progressbar" style="width: 89%" aria-valuenow="89" aria-valuemin="0" aria-valuemax="100"></div>
                      </div>
                      <small>Mobile Template</small>
                      <div class="progress mb-3" style="height: 5px">
                        <div class="progress-bar bg-primary" role="progressbar" style="width: 55%" aria-valuenow="55" aria-valuemin="0" aria-valuemax="100"></div>
                      </div>
                      <small>Backend API</small>
                      <div class="progress mb-3" style="height: 5px">
                        <div class="progress-bar bg-primary" role="progressbar" style="width: 66%" aria-valuenow="66" aria-valuemin="0" aria-valuemax="100"></div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>



            </div>
          </div>

        </div>
    </div>
   
  </section>
</template>

<script>
export default {
  name: 'HeroSection'
}
</script>
<style scoped>
.hero {
  text-align: center;
  padding: 100px 0;
  background-image: url(https://w0.peakpx.com/wallpaper/834/159/HD-wallpaper-anime-aesthetic-aesthetic-anime.jpg);

}
</style>
