<template>
  <div id="app">
    <Header />
    <Banner />
    <About />
    <Testimonials />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header"
import Banner from "./components/Banner"
import About from "./components/about"
import Testimonials from "./components/testimonials"
import Contact from "./components/contact"
import Footer from "./components/footer"

export default {
  name: "App",
  data(){
    return{

    }
  },
  components: {
    Header,
    Banner,
    About,
    Testimonials,
    Contact,
    Footer
  }
};
</script>

