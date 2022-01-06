<template>
  <b-container fluid>
    <b-row align-h="center" class="main-row">
      <b-col xl="3" lg="3">
        <b-img thumbnail fluid src="https://picsum.photos/250/250/?image=54" alt="Image 1"></b-img>
      </b-col>
      <b-col xl="7" lg="7">
        <b-container class="right-section">
          <b-row>
            <b-col>
              <h1>Johnny Test <i id="title">(2005–2014)</i></h1>
              
            </b-col>
          </b-row>
          <b-row>
            <b-col>
              <p>The adventures of average suburban boy Johnny Test, who wittingly plays test subject for his
              genius twin sisters' various experiments, reluctantly ﬁghting evil villains in the process.</p>
            </b-col>
          </b-row>
          <b-row>
            <b-col cols="12">
              <p class="details"><span class="key-word">Genre: </span>
              Animation, Action, Adventure, Comedy, Drama, Family, Sci-Fi
              </p>
            </b-col>
            <b-col cols="12">
              <p class="details"><span class="key-word">Actors: </span>
              James Arnold Taylor, Maryke Hendrikse, Lee Tockar, Ashleigh Ball
              </p>
            </b-col>
            <b-col cols="12">
              <p class="details"><span class="key-word">Director: </span>
              N/A
              </p>
            </b-col>
            <b-col cols="12">
              <p class="details"><span class="key-word">Writers: </span>
              1 win & 5 nominations.
              </p>
            </b-col>
            <b-col cols="12">
              <p class="details"><span class="key-word">Type: </span>
              Series
              </p>
            </b-col>
            <b-col cols="12">
              <p class="details"><span class="key-word">Awards: </span>
              1 win & 5 nominations.
              </p>
            </b-col>
            <b-col cols="12">
              <p class="details"><span class="key-word">language: </span>
              English
              </p>
            </b-col>
            <b-col cols="12">
              <p class="details"><span class="key-word">Released: </span>
              01 Jan 2005
              </p>
            </b-col>
          </b-row>
          <b-row align-h="center">
            <b-col cols="3">
              <p class="rating">IMBD Ratings</p>
                <star-rating 
                  @rating-selected ="setRating"
                  :increment="0.1"
                  :max-rating="10" 
                  :star-size="13">
                </star-rating>
            </b-col>
            <b-col cols="2">
              <p class="rating">IMBD Votes</p>
              <p>6,419</p>
            </b-col>
          </b-row>
          <b-row align-h="between">
            <b-col cols="3">
              <b-button @click="$router.go(-1)" variant="primary">&#8249; Back</b-button>
            </b-col>
            <b-col cols="3">
              <star-rating 
                @rating-selected ="setRatingSingle"
                :increment="1"
                :max-rating="1" 
                :star-size="50">
              </star-rating>
              <span>
              Note:<br>
              Add/Remove<br>
              from favorites
              </span>
            </b-col>
          </b-row>
        </b-container>
      </b-col>
    </b-row>
    
  </b-container>
</template>

<script>
import StarRating from 'vue-star-rating'
export default {
  components: {
    StarRating
  },
    data() {
      return {
        rating: 0,
        singleRating: 0
      }
  },
  methods: {
    setRating(rating) {
      this.rating= rating;
    },
    setRatingSingle(rating) {
      this.singleRating = rating;
    }
  }

}
</script>

<style scoped>
  .container-fluid {
    background-color: #fff;
  }

  .main-row {
    padding-top: 20px;
  }

  h1 i {
    font-size: 20px;
    margin-left: 10px;
    
  }

  .right-section{
    padding-right: 0;
  }

  .key-word {
    font-weight: bold;
  }
  
  button {
    width: 145px;
    height: 35px;
  }

  .rating {
    margin-bottom: 0px;
  }

</style>