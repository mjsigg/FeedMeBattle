<template>

<div>
    <div class="parent">

        <header>
            <h2 class="company-name">Phat Eatery || Insert Logo here</h2>
        </header>

        <article class="left-side-main" contenteditable>
            <section>
                Left Sidebar || Tons of discounts throughout the month of November!
            </section>
        </article>

        <article class="middle-main" contenteditable>
            <section> 
                Right Sidebar
                Main Column|| Free merch to the first 50 veterans!  Bring ID!
            </section>
        </article>

        <article class="right-side-main" contenteditable>
            <section> 
                Right Sidebar
                RightSidebar || TESTING THIS BADBOY OUT SON!!!!!!!!!!!!!!!!!!
            </section>
        </article>

        <footer class="footer">
            <section>Keeping this in now as a placeholder.  Might need some sort of gap fpr spacing?</section>
        </footer>
        
    </div>
        <article class="sidebar-parent">
            <section class="sidebar"><h3>yo man testing this shit out</h3></section>
                <p class="sidebar-remainder">Sidebar remainder</p>
        </article>
</div>
</template>

<script>
export default {

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