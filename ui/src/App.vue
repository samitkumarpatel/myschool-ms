<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">
        <img src="./assets/school.png" alt="no logo">
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link class="nav-link" to="/">dashboard</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/admin">admin</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/user">user</router-link>
          </li>
        </ul>
        <form class="d-flex">
          <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success" type="submit">Search</button>
        </form>
      </div>
    </div>
  </nav>

  <router-view/>

  <footer>
    <small>
      <p>@ all right received!</p>
    </small>
  </footer>
</template>

<style>
nav {
  margin-bottom: 30px;
  margin-top: 10px;
}

img {
  width: 35px;
}
footer {
  margin-top: 150px;
  color: gray;
}
</style>
