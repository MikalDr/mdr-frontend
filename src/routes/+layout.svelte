<script>
    import "../style.scss"
    import { page } from '$app/stores';
    import { derived } from 'svelte/store';

    const isProjectsPage = derived(page, $page => $page.url.pathname === '/projects');
    const isContactPage = derived(page, $page => $page.url.pathname === '/contact');
    const isAboutPage = derived(page, $page => $page.url.pathname === '/about');
    const isHome = derived(page, $page => $page.url.pathname === '/');
    const isNotHome = derived(page, $page => $page.url.pathname !== '/');
</script>

<div id="mainbox" class="mainbox" class:main-box-gone={$isNotHome}>
    <div class="main-section">
        <h1>Hi! I am Mikal!</h1>
        <p>I am a programmer, that is currently taking a joint Master's Degree in Software Engineering at UiB and HVL.</p>
        <p>Most of my code never sees the light of day, but i do enjoy making them! I enjoy writing code in Rust and C#</p>
        <p>but do also enjoy trying new frameworks and other programming languages, on occasion.</p>
    </div>
</div>

<div class="navbar">
    <ul class="header-buttons">
        <li><a href="/" class:navbar-button-active={$isHome}>Home</a></li>
        <li><a href="/about" class:navbar-button-active={$isAboutPage}>about</a></li>
        <li><a href="/projects" class:navbar-button-active={$isProjectsPage}>projects</a></li>
        <li><a href="/contact" class:navbar-button-active={$isContactPage}>contact</a></li>
    </ul>
</div>

<slot></slot>

<style>
    .mainbox {
        margin: 2rem;
        width: 100%;
        height: 10rem;
        left: 0;
        transition: all 1s;
    }

    a {
        font-size: 1.5rem;
    }

    .main-box-gone {
        transform: scaleY(0);
        height: 0;
        margin-top: 0;
        margin-bottom: 0;
        opacity: 0;
    }    

</style>