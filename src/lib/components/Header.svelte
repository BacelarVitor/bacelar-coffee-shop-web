<script lang="ts">
    let toggle = false;

    function toggleMenu() {
        toggle = !toggle;
    }
</script>
<header>
    <nav class="navbar" role="navigation" aria-label="main navigation">
        <div class="navbar-brand">
            <a href="/" role="button" class="navbar-item">
                <!-- <img src="" width="122" height="28"> -->
                Bacelar coffee Shop
            </a>
            <!-- svelte-ignore a11y-missing-attribute -->
            <!-- svelte-ignore a11y-interactive-supports-focus -->
            <!-- svelte-ignore a11y-click-events-have-key-events -->
            <a role="button" class="navbar-burger {toggle ? 'is-active' : ''}" aria-label="menu" on:click={toggleMenu} aria-expanded="false" data-target="nav-menu">
                <span aria-hidden="true"></span>
                <span aria-hidden="true"></span>
                <span aria-hidden="true"></span>
            </a>
        </div>

        <div id="nav-menu" class="navbar-menu {toggle ? 'is-active' : ''}">
            <div class="navbar-end">
                <a href="google.com" class="navbar-item">fon</a>
                <a href="google.com" class="navbar-item">flin</a>
                <a href="google.com" class="navbar-item">lin</a>
            </div>
        </div>
    </nav>
</header>
