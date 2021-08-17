<template>
    <div class="parent">
        <title>Phat Eatery</title>
        <header class="header">
           <h2 class="company-name">Phat Eatery</h2>
        </header>
        <div class="left-side-main" contenteditable>Left Sidebar</div>

        <main class="middle-main" contenteditable> 
            <div class="ram-layout">
                <div class>Free merchandise on Friday's!
                    <p>Throughout the month Septemember we are giving out free merch to the first 10 veterans that show their ID.  Thank you for your service!</p>
                </div>

                <div>
                    <p>Our countdown to Veteran's Day kicks off in the beginning of September with a 10% discount on appetizers, a free drink, and 5% match of total to Combined Arms!</p>
                </div>
                <div class>3</div>
                <div class>4</div>
            </div>
        </main>
    
        <div class="right-side-main" contenteditable>Right Sidebar</div>
        <footer class="footer">Footer</footer>
          
    </div>
</template>

<script>
export default {

}
</script>

<style>
  .parent {
    display: grid;
    grid-template-columns: auto 1fr auto / auto 1fr auto;
  }
  
  .header {
    grid-column: 1/4;
    padding: 2rem;
    background-color: brown;
  }

  .left-side-main{
    grid-column: 1 / 2;
    background-color: yellow;
  }

  .middle-main {
    grid-column: 2/3;
    background-color: grey;
  }

  .right-side-main {
    grid-column: 3/4;
    background-color: red;
  }

  .footer{
    grid-column: 1 / 4;
    background-color: green;
  }

  .company-name{
    background-color: yellowgreen;
    text-align: center;
      
  }
  .ram-layout {
    display: grid;
    grid-gap: 1rem;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  }

</style>