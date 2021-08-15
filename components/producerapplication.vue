<template>
    <div class="container">  
        <form>
            <h2> Producer Application</h2>
            <label for="contactName">Point of Contact:</label>
                <input class="categoryInput" type="contactName" required v-model="contactName">
            <label for="phone">Phone:</label>
                <input class="categoryInput" type="phone" required v-model="phone">
            <label for="email">Email:</label>     
                <input class="categoryInput" type="email" required v-model="email">
        <div>
            <label for="=socialMedia">Please provide any links to sites/social media you would like to us to link:</label>
                <textarea class="textareaInput" type="socialMedia" v-model="socialMedia"></textarea>
        </div>

        <div>
            <label></label>
                <span class="categorySpan">Below are some examples and notes to consider when participating in the program.  The examples are merely,</span> <span>
                    so please feel free to brainstorm below any ideas you'd like to share</span>
                <textarea class="textareaInput" type="socialMedia" v-model="socialMedia"></textarea>
        </div>

        <div>
             <input class="button" type="submit" value="Submit">
        </div>
        </form>

    <p> {{contactName}}</p>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>

.container {
    display: flex;
    background-color: turquoise;
}

.categoryInput{
    background-color: lightgrey;
    width: 50%;
    height: 25px;
    display: flex;
    border: 5px black;
    margin:5px;  
}

.textareaInput {
    background-color: lightgrey;
    width: 50%;
    height: 250px;
    display: flex;
    border: 5px black;
    padding: 2px;
    margin:5px;
}

.categorySmallInput {
    background-color: lightgrey;
    width: 10%;
    height: 25px;
    display: flex;
    border: 5px black;
    margin:2px;
}

.categorySpan {
    display: block;
}

.button {
    margin: 30px;
    background-color: #39495c;
    border-radius: 5px;
    font-size: 18px;
    width: 160px;
    height: 60px;
    color: white;
    text-align: center;
    cursor: pointer;

}
</style>>

data() {
    return {
        contactName:'',
        phone:'',
        email:'',
        socialMedia: [],
    }
}