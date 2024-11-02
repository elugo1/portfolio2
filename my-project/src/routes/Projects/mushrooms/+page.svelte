<script>
    import ImgExp from "../../../components/ImgExp.svelte";
</script>

<div class="container" >
    <h1  style="color: black; font-size: 2em;"> Cemetery Spore Prints</h1>
    <p text-lg mb-4 style="max-width: 60%; padding-bottom: 20px;">
        In this project I created a typology of spore prints from wild mushrooms foraged in Homewood Cemetery Pittsburgh, and displayed them with the names of the buried they were found closest to. The goal being to create a posthumous portrait of the individual buried. This project was done in the <a href="https://courses.ideate.cmu.edu/60-461/f2022/index.html" style="color: blue; text-decoration: underline;">Experimental Capture</a> course taught by Golan Levin and Nica Ross    
    </p>
    <ImgExp imgurl={{ thumbnail: '../spore_prints/full_prints.png', full: '../spore_prints/full_prints.png' }} />
    <p text-lg mb-4 style="max-width: 60%;">
        Spore printing is performed by cutting off the stem, covering the mushroom cap, and letting it sit for 2-24 hours as the spores fall. Spore printing is mainly used by foragers for mushroom-identification, as the color of a mushroom’s spores may be one of the only differences between an edible mushroom and a poisonous lookalike. Spore printing is also a tool for archiving and preservation as the spores can lay dormant for years in a well-maintained spore print, ready to restart the life cycle of the fungus.
    </p>
    <div class="frame-grid">
        <img src="/spore_prints/slicing_shroom.gif" alt="slicing_shroom.gif" />
        <img src="/spore_prints/grave_shrooms.jpg" alt="grave_shroom" />
    </div>
    <img src="/spore_prints/closeup_1.png" alt="closeup_1" style ="padding-top:20px; max-width:100%;"  />
    <img src="/spore_prints/closeup_2.png" alt="closeup_1" style ="padding-top:20px; max-width:100%;"  />

</div>

<style>
    .container {
        display: flex;
        flex-direction: column;   /* Stack elements vertically */
        justify-content: center;  /* Center content horizontally */
        align-items: center;      /* Center content vertically */
        width: 100%;              /* Full width of the page */
        max-width: 100%;          /* Override inherited max-width */
        height: 100%;
    }

    .frame-grid {
        display: grid;
        grid-template-columns: repeat(2, 1fr); /* 2 equal-width columns */
        gap: 20px;                             /* Space between images */
        max-width: 60%;                        /* Optional: control overall grid width */
        margin-top: 20px;
    }

    .frame-grid img {
        width: 100%;       /* Make images responsive within their grid cells */
        height: auto;      /* Maintain aspect ratio */
        object-fit: cover; /* Optional: ensures consistent cropping if images are different aspect ratios */
    }
</style>
