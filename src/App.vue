<template>
  <div class="page-container">
    <div class="page">
      <div class="container g-0">
        <div class="row m-0">
          <div class="col-12 col-md-4 scrollable side-column" >
            <SideColumn/>
          </div>
          <div class="col-12 col-md-8 px-4 scrollable">
            <MainContent/>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import SideColumn from "./components/SideColumn.vue";
import MainContent from "./components/MainContent.vue";

export default {
  name: 'App',
  components: {
    SideColumn,
    MainContent
  }
}
</script>

<style lang="scss">
@import "@/scss/custom";

body {
  background-color: $dark;
}

.page-container {
  display: flex;
  align-items: center;
  justify-content: center;
}

.page {
  background-color: white;
  border-radius: 5px;
  max-width: 768px;
}

.side-column {
  position: relative;
  background-color: $secondary;
}

@include media-breakpoint-up(md) {
  .page {
    max-height: calc(100vh - 40px);
    margin-top: 20px;
    margin-bottom: 20px;
    -webkit-box-shadow: #181818 20px 20px 20px;
    -moz-box-shadow: #181818 20px 20px 20px;
    box-shadow: #181818 20px 20px 20px;
  }

  .scrollable {
    overflow-y: auto;
    max-height: calc(100vh - 40px);
    -ms-overflow-style: none;
    scrollbar-width: none;
  }

  .scrollable::-webkit-scrollbar {
    display: none;
  }

  .side-column {
    border-top-left-radius: 5px;
    border-bottom-left-radius: 5px;
  }
}

</style>
