<script lang="ts">
    import cards from "./cards.json";
    let rcounter = 0
    let fcounter = 0
</script>


<header>
    Flashcards
</header>
<body>
<div class = "flashcard-space">
    <div class="first-row">
        <div class= "arrow">←</div>
        <div class= "card"> and now I actually need to program B') </div>
        <div class= "arrow">→</div>
    </div>
    <div class= "second-row">
        <div class= "RF">
            ⭕︎ {rcounter}
        </div>
        <div class= "RF">
            ✕ {fcounter}
        </div>
    </div>
    <div class= "instructions">
        If I figure this out: <br>
        ← previous card, → next card <br>
        ↑ correct, ↓ wrong
    </div>
</div>
</body>

<style lang="scss">
    
    header {
        text-align: center;
        padding: 1em;
        font-size: 3em;
        margin-bottom: 1rem;
    };

    
    body {
        background-color: rgba(51,33,49,255);
        color: rgb(251,241,238);
    }

    .flashcard-space {
        max-height: 30rem;

        display: flex;
        flex-wrap: wrap;

        justify-content: center;
        align-items: center;
        
    };

    .first-row {
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }


    .card {
        max-width: 30rem;
        max-height: 30rem;
        width: 30rem;
        height: 30rem;
        padding: 0.5rem;
        border-radius: 1em;

        display: flex;
        justify-content: center;
        align-items: center;

        text-align: center;

        color: rgb(56,36,54);
        background-color: rgb(251,241,238);


        font-size: 2em;
    }

    .arrow {
        padding: 0.5em;
        font-size: 3em;
    }

    .second-row {
        padding: 0.5em;
        font-size: 3em;

        
        display: flex;
        flex-wrap: wrap;

        width: 100%;
        justify-content: center;
        align-items: center;
    }

    .RF{
        margin: 2rem;
        padding: 1rem 2rem 1rem 2rem;
        background-color:rgb(81, 49, 78);
        border-radius: 1rem;
    }

    .instructions {
        font-size:1rem;
        text-align: center;
    }

</style>
