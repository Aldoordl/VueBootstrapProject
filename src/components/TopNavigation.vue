<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-white py-3">
      <div class="container px-5">
          <RouterLink class="navbar-brand" to="/"><span class="fw-bolder text-primary">VueJs</span></RouterLink>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation"><span class="navbar-toggler-icon"></span></button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
              <ul class="navbar-nav ms-auto mb-2 mb-lg-0 small fw-bolder">
                  <li class="nav-item">
                    <RouterLink class="nav-link" to="/">Home</RouterLink>
                  </li>
                  <li class="nav-item">
                    <RouterLink class="nav-link" to="/project">About</RouterLink>
                  </li>
                  <li class="nav-item">
                    <RouterLink class="nav-link" to="/kalkulator">Playground</RouterLink>
                  </li>
              </ul>
          </div>
      </div>
  </nav>
</template>