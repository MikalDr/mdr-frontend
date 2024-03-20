<script>
    const projects = [
        {"title": "FeedApp",
        "content": "This is a project created in relation to the subject Dat250 at HVL. It is a voting application where user can create polls on different subjects"},
        {"title": "TryBlocking - Rust",
        "content": "TryBlocking is a game I created during a gamejam. This is a project centered around recreating it in Bevy, a game engine for Rust."},
        {"title": "Battle-System",
        "content": "Battle-system is a haskell project created in relation to the subject INF221 at UiB. The project is essentially creating a pokemon battle system in Haskell"},
    ]
</script>

<div class="mainbox">
    <div>
        <h1>Projects</h1>
        <div class="project-articles">
            {#each projects as p}
                <div class="articles">
                    <h3>{p.title}</h3>
                    <p>{p.content}</p>
                    <div><a href="">read more</a> <a href="">github</a></div>
                </div>
            {/each}
        </div>
    </div>
</div>