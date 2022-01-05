<template>
  <b-container fluid >
    <b-row align-h="center">
      <b-col xl="3" lg="3" class="left-section">
          <b-form @submit="onSubmit" @reset="onReset" >
            <b-form-group
              id="input-group-1"
            >
              <p>Name/Title:</p>
              <b-form-input
                id="input-1"
                v-model="form.name"
                type="text"
                placeholder="Name/Title"
                required
              ></b-form-input>
            </b-form-group>

            <b-form-group id="input-group-2" >
              <p>Year:</p>
              <b-form-input
                id="input-2"
                v-model="form.year"
                type="number"
                placeholder="Year"
                required
              ></b-form-input>
            </b-form-group>

            <b-form-group id="input-group-3" >
              <p>Type:</p>
              <b-form-input
                id="input-3"
                v-model="form.type"
                type="text"
                placeholder="Type"
                required
              ></b-form-input>
            </b-form-group>
            

             <b-button type="submit" class="btn-search">Search</b-button>
          </b-form>
      </b-col>
      <b-col xl="7" lg="7" class="right-section">
        <b-container>
          <b-row class="display-nav">
            <b-col style="text-align: center;">
              <b-link href="/">Grid</b-link>
              <b-link href="/about">List</b-link>
            </b-col>
          </b-row>
          <b-row align-h="center">

            <b-col xl="3" lg="3" class="m-3">
              <b-card
                  title="Anabel"
                  img-src="https://picsum.photos/600/300/?image=25"
                  img-alt="Image"
                  img-top
                  tag="article"
                  style="max-width: 20rem;"
                  class="mb-2 text-center"
                >
                  <b-card-text>
                    2021 - Horror
                  </b-card-text>

                  <!-- <b-button href="#" variant="primary">Go somewhere</b-button> -->
                </b-card>
              </b-col>

              <b-col xl="3" lg="3" class="m-3">
              <b-card
                  title="Anabel"
                  img-src="https://picsum.photos/600/300/?image=25"
                  img-alt="Image"
                  img-top
                  tag="article"
                  style="max-width: 20rem;"
                  class="mb-2 text-center"
                >
                  <b-card-text>
                    2021 - Horror
                  </b-card-text>

                  <!-- <b-button href="#" variant="primary">Go somewhere</b-button> -->
                </b-card>
              </b-col>

              <b-col xl="3" lg="3" class="m-3">
              <b-card
                  title="Anabel"
                  img-src="https://picsum.photos/600/300/?image=25"
                  img-alt="Image"
                  img-top
                  tag="article"
                  style="max-width: 20rem;"
                  class="mb-2 text-center"
                >
                  <b-card-text>
                    2021 - Horror
                  </b-card-text>

                  <!-- <b-button href="#" variant="primary">Go somewhere</b-button> -->
                </b-card>
              </b-col>

              <b-col xl="3" lg="3" class="m-3">
              <b-card
                  title="Anabel"
                  img-src="https://picsum.photos/600/300/?image=25"
                  img-alt="Image"
                  img-top
                  tag="article"
                  style="max-width: 20rem;"
                  class="mb-2 text-center"
                >
                  <b-card-text>
                    2021 - Horror
                  </b-card-text>

                  <!-- <b-button href="#" variant="primary">Go somewhere</b-button> -->
                </b-card>
              </b-col>

              <b-col xl="3" lg="3" class="m-3">
              <b-card
                  title="Anabel"
                  img-src="https://picsum.photos/600/300/?image=25"
                  img-alt="Image"
                  img-top
                  tag="article"
                  style="max-width: 20rem;"
                  class="mb-2 text-center"
                >
                  <b-card-text>
                    2021 - Horror
                  </b-card-text>

                  <!-- <b-button href="#" variant="primary">Go somewhere</b-button> -->
                </b-card>
              </b-col>

              <b-col xl="3" lg="3" class="m-3">
              <b-card
                  title="Anabel"
                  img-src="https://picsum.photos/600/300/?image=25"
                  img-alt="Image"
                  img-top
                  tag="article"
                  style="max-width: 20rem;"
                  class="mb-2 text-center"
                >
                  <b-card-text>
                    2021 - Horror
                  </b-card-text>

                  <!-- <b-button href="#" variant="primary">Go somewhere</b-button> -->
                </b-card>
              </b-col>

              
              
          </b-row>
        </b-container>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  name: 'Home',
  props: {
    msg: String
  },
  data() {
    return{
      form: {
          name: '',
          year: '',
          type: ''
        },
    }
  }
}
</script>

<style scoped>
  .container-fluid {
    background-color: white;
  }

  .col-xl-3{
    padding: 0 !important;
  }

  .form-group {
    margin: 20px 0;
  }

  form p {
    font-size: 20px !important;
    margin-bottom: 10px;
  }

  .btn-search {
    background-color: #00BFFF !important;
    border: none;
    width: 100%;
    height: 45px;
    font-size: 20px;
    border-radius: 10px;
    margin-top: 20px;
  }

  input {
    height: 45px;
    border-radius: 10px;
  }

  ::placeholder {
    font-size: 18px;
  }
  .display-nav {
    margin: 20px 0;
  }

  .display-nav a {
    text-decoration: none !important;
    margin: 15px;
    color: #000;
    font-size: 20px;
    padding-bottom: 4px;
  }

  a:hover {
    border-bottom: 1.7px solid rgba(0, 0, 0, 0.8);
  }

  /* //Todo porpaviti */
  .left-section {
    margin-right: 30px;
  }

  

</style>