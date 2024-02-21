<script>
    const projects = [
        {"title": "Test",
        "content": "This is a test project. I would like this to look neat. and not bad"},
        {"title": "Test",
        "content": "This is a test project. I would like this to look neat. and not bad"},
        {"title": "Test",
        "content": "This is a test project. I would like this to look neat. and not bad"},
    ]
</script>

<div class="mainbox">
    <div>
        <h1>This is my current projects</h1>
        <div class="project-articles">
            {#each projects as p}
                <div class="articles">
                    <h3>{p.title}</h3>
                    <p>{p.content}</p>
                </div>
            {/each}
        </div>
    </div>
</div>