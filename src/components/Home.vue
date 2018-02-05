<template>
  <div class="texto">
    <span>{{ name }}</span>
    Desenvolvedor de sistemas apaixonado pelo que faz
    <a :href="github">GitHub</a>
    <a :href="gitlab">GitLab</a>
    <a :href="linkedin"><img src="../assets/Logo-White-128px-TM.png" width="150"/></a>
    <a class="email" href="mailto:contato@fucazu.com">contato@fucazu.com</a>
  </div>
</template>

<script>

export default {
  name: 'Home',
  data () {
    return {
      name: 'Rafael Sanches',
      github: 'https://github.com/fucazu',
      gitlab: 'https://gitlab.com/fucazu',
      linkedin: 'https://www.linkedin.com/in/rafaelsanchesdev/'
    }
  }
}
</script>

<style lang="scss" scoped>
.texto {
  height: 100%;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: nowrap;
  color: white;
  flex-direction: column;
  margin: auto;
  text-align: center;
  span {
    font-size: 50px;
  }
  a {
    text-decoration: none;
    background-image: none;
    color: white;
    min-width: 150px;
    font-size: 43px;
    font-family: 'Roboto Condensed', sans-serif;
    &.email {
      font-size: 30px;
    }
  }
}
</style>
