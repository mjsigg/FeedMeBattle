<template>

<div>

    <div class="parent">
        <header>
            <h2 class="company-name">
                {{companyName}} <img src="phat eatery logo.jpeg" alt="Company Logo">
            </h2>
        </header>

        <article class="left-side-main section-padding" contenteditable>
            <section>
                Left Sidebar || Tons of discounts throughout the month of November!
            </section>
        </article>

        <article class="middle-main section-padding" contenteditable>
            <section> 
                Middle Sidebar
                Main Column|| Free merch to the first 50 veterans!  Bring ID!
            </section>
        </article>

        <article class="right-side-main section-padding" contenteditable>
            <section> 
                Right Sidebar
                RightSidebar || TESTING THIS BADBOY OUT SON!!!!!!!!!!!!!!!!!!
            </section>
        </article>


        
    </div>
        <article class="sidebar-parent">
            <section class="sidebar">
                <h3>Menu items</h3>
                <p>beef rendang</p>
                <p>galngal</p>
                ginger
            </section>
                <section class="sidebar-remainder">
    <client-only>
        <vue-pdf class='' :src="src" :page="1" @num-pages="pdfPageCount = $event"></vue-pdf>
        <div v-if="pdfPageCount > 1">
            <div v-for="(pageNum, index) in pdfPageCount " :key="index">
                <vue-pdf class="your-pdf-class" :src="src" :page="pageNum" v-if="pageNum > 1"></vue-pdf>
            </div>
        </div>
    </client-only>
                </section>
        </article>
</div>

</template>

<script>

export default {
        components: {
        pdf
    },

    data() {
        return {
            companyName: 'Phat Eatery',
            companyLogo: 'Phat Eatery Logo.jpeg',
            menuPDF: 'phat-menu.pdf',
            src: 'https://img1.wsimg.com/blobby/go/cc9b23cf-8ed7-4c72-a7ab-7ac80deb140d/downloads/7-10%20Dinner.pdf?ver=1629149791217',
            pdfPageCount: 0,
		}
	},
}
</script>

<style>

  header {
    grid-column: 1/4;
    padding: 2rem;
    background-color: brown;
  }

  .company-name{
    background-color: yellowgreen;
    text-align: center;   
  }

  .parent {
    display: grid;
    grid-template-columns: auto 1fr auto / auto 1fr auto;
  }
  
  .left-side-main {
    grid-column: 1 / 2;
    background-color: yellow;
  }

  .section-padding {
      padding: 2rem;
  }

  .middle-main {
    grid-column: 2 / 3;
    background-color: grey;
  }

  .right-side-main {
    grid-column: 3 / 4;
    background-color: red;
  }

  footer{
    grid-column: 1 / 4;
    background-color: turquoise;
  }

  .sidebar-parent{
  display: grid;
  grid-template-columns: minmax(150px, 65%) 1fr;
  padding: 0;
  margin: 0;
}

  .sidebar {
  height: 100vh;
  background: lightpink;
  font-size: 2rem;
  text-align: center;
}

.sidebar-remainder{
  grid-template-columns: minmax(150px, 65%) 1fr;
  padding: 0;
  margin: 0;
  background-color: gray;
  }


</style>