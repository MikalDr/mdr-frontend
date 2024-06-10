<div class="mainbox">
    <h1>How to contact me</h1>
    <div class="contactinfo">
        <div class="contactbox">
            <img src="https://avatars.githubusercontent.com/u/105053235?v=4" alt="githubIcon" class="responsive-image-small">
            <div class="infobox">
                <h2>GitHub</h2>
                <a href="https://github.com/MikalDr"><p>MikalDr</p></a>
            </div>
        </div>

        <div class="contactbox">
            <img src="https://i.pinimg.com/originals/84/6a/03/846a03c6760f83f3a0e92609bca9cebf.jpg" alt="githubIcon" class="responsive-image-small">
            <div class="infobox">
                <h2>Email</h2>
                <a href="mailto:mikal-dr@hotmail.com"><p>Mikal-dr@hotmail.com</p></a>
            </div>
        </div>

        <div class="contactbox">
            <img src="/In-White-72@2x.png" alt="linkedInLogo" class="responsive-image-small">
            <div class="infobox">
                <h2>LinkedIn</h2>
                <a href="https://no.linkedin.com/in/mikal-drivenes-a1339b23a"><p>Mikal Drivenes</p></a>
            </div>
        </div>

    </div>
</div>

<style lang="scss">
    .mainbox {
        display: flex;
        flex-direction: column;
        margin: 2rem;
        align-items: center;
        gap: 1rem;
        }
    .contactinfo {
        display: grid;
        grid-template-columns: auto auto auto;
        column-gap: 1rem;
        row-gap: 1rem;
    }
    .contactbox {
        display: flex;
        flex-direction: column;
        align-items: center;
        //background-color: rgb(70, 22, 16);
        border: solid 2px white;

        width: 20rem;
        padding: 1rem;
        border-radius: 2rem;
        gap: 2rem;

        a {
            color: white;
        }
    }
    .responsive-image-small {
        max-width: 5rem;
        min-width: 150px;
        height: auto;
        border-radius: 30%;
    }
    .infobox {

    }
</style>