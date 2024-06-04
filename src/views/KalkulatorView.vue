<script setup>
import { ref } from 'vue';

const tulisan = ref('Welcome to My Playground');
const aplikasi = ref('Summation Calculator');
const nama = ref("John Doe");
const inputAngkaSatu = ref(null);
const inputAngkaDua = ref(null);
const hasil = ref(null);

const proses = () => {
  const angkaSatu = parseInt(inputAngkaSatu.value);
  const angkaDua = parseInt(inputAngkaDua.value);

  hasil.value = angkaSatu + angkaDua;
};

</script>

<template>
  <section class="pt-5">
      <div class="container px-5">
          <div class="bg-light rounded-4 py-5 px-4 px-md-5">
              <div class="text-center mb-5">
                  <div class="feature bg-primary bg-gradient-primary-to-secondary text-white rounded-3 mb-3"><i class="bi bi-people"></i></div>
                  <h1 class="fw-bolder">{{ tulisan }}, {{ nama }}👋</h1>
                  <p class="lead fw-normal text-muted mb-0">Let's try typing your name!</p>
              </div>
              <div class="row gx-5 justify-content-center">
                  <div class="col-lg-8 col-xl-6">
                      <form id="contactForm">
                          <div class="form-floating mb-3">
                              <input class="form-control" id="name" type="text" placeholder="John Doe" data-sb-validations="required" v-model="nama" />
                              <label for="name">Your Name</label>
                              <div class="invalid-feedback" data-sb-feedback="name:required">A name is required.</div>
                          </div>
                      </form>
                  </div>
              </div>
          </div>
      </div>
  </section>
  <section class="py-5">
      <div class="container px-5">
          <div class="bg-light rounded-4 py-5 px-4 px-md-5">
              <div class="text-center mb-5">
                  <div class="feature bg-primary bg-gradient-primary-to-secondary text-white rounded-3 mb-3"><i class="bi bi-calculator"></i></div>
                  <h1 class="fw-bolder">{{ aplikasi }}</h1>
                  <p class="lead fw-normal text-muted mb-0">Let's use my calculator!<br>Result: {{ hasil }}</p>
              </div>
              <div class="row gx-5 justify-content-center">
                  <div class="col-lg-8 col-xl-6">
                      <form id="contactForm">
                          <div class="form-floating mb-3">
                              <input class="form-control" id="one" type="number" placeholder="1234567890" data-sb-validations="required" v-model="inputAngkaSatu" />
                              <label for="name">Number One</label>
                              <div class="invalid-feedback" data-sb-feedback="one:required">A number one is required.</div>
                          </div>
                          <div class="form-floating mb-3">
                              <input class="form-control" id="two" type="number" placeholder="1234567890" data-sb-validations="required" v-model="inputAngkaDua" />
                              <label for="email">Number Two</label>
                              <div class="invalid-feedback" data-sb-feedback="two:required">An number two is required.</div>
                          </div>
                          <div class="d-grid"><button class="btn btn-primary btn-lg" id="submitButton" type="button" @click="proses">Calculated</button></div>
                      </form>
                  </div>
              </div>
          </div>
      </div>
  </section>
</template>
