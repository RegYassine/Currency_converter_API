<template>
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
                <div class="container-fluid">
                  <!--props WITH VARIABLE NAME AND TYPE, BALISE IN app.vue AND WHERE TO USE IT-->
                  <a class="navbar-brand" href="#">{{title}}</a>
                  <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarColor01" aria-controls="navbarColor01" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                  </button>

                  <div class="collapse navbar-collapse" id="navbarColor01">
                    <ul class="navbar-nav me-auto">
                      <li class="nav-item">
                        <!--CHANGE a TO router-link AND href TO to-->
                        <router-link class="nav-link active" to="/">Home
                          <span class="visually-hidden">(current)</span>
                        </router-link>
                      </li>
                      <li class="nav-item">
                        <router-link class="nav-link" to="add_contact">Add Contact</router-link>
                      </li>
                    </ul>
                  </div>
                </div>
    </nav>
</template>

<script>
    export default {
        name: 'MyHeader',
        props: {
            title: String
        }
    }
</script>