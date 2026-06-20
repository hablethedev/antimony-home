<script>
    import Navbar from '$lib/navbar.svelte';
    import Button from '$lib/button.svelte';
</script>

<Navbar />


        <div class="thingy">
            <h1>Antimony Desktop</h1>
            <p>Antimony Desktop is a new application that ports the Antimony website onto desktops.</p>

            <div class="center-wrapper-thingy">
                <Button
                icon="download.svg" // lucide my wife :3
                label="Download" 
                highlighted={true} 
                link="https://github.com/antimony-editor/editor/releases" 
        />
    </div>
    <small>Antimony Desktop is currently in public alpha. <a href="https://github.com/antimony-editor/editor/issues">Your feedback would help us!</a></small>

    <div class="desktop-screenshot">
        <img src="desktop.png" alt="A screenshot of Antimony Desktop">
    </div>    
</div>

<main class="features">
    <section class="all-sections">
        <h2>Features</h2>
        <ul class="all-lists">
            <li>
                <div class="feature-thingyyy">
                <img src="wifi-off.svg" alt="Wifi Disabled">
                <p>Works offline</p>
                </div>
                <p>Out and about? A power outage is happening? Antimony Desktop works even when your not connected to the internet!</p>
            </li>
        </ul>
    </section>
</main>

<div class="footer">
    <p>Made with &lt;3 by the Antimony Team</p>
        <div class="footer2">
        
        <div class="footer-column">
            <h4>Website</h4>
            <a href="https://editor.antimony.cc" style="color: white;"><p>Editor</p></a> 
            <a href="desktop" style="color: white;"><p>Desktop App</p></a> 
            <a href="credits" style="color: white;"><p>Credits</p></a>
            <a href="https://github.com/antimony-editor" style="color: white;"><p>GitHub</p></a>
        </div>

        <div class="footer-column">
            <h4>Community</h4>
            <a href="https://github.com/antimony-editor/antimony-home/issues" style="color: white;"><p>Report an issue</p></a>
            <a href="https://www.youtube.com/channel/UCuC_CpmCqhKV6g0I33s6PJQ" style="color: white;"><p>YouTube</p></a>
            <a href="https://discord.gg/CeJVMHXhCP" style="color: white;"><p>Discord</p></a>
        </div>
        
    </div>
</div>

<style>
    .desktop-screenshot {
        display: flex;
        justify-content: center;
        gap: 20px;
        padding: 10px;
    }
    .desktop-screenshot img {
        border-radius: 15px;
        width: 100%;
        max-width: 600px;
        height: auto;
    }
    
    .features {
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
    }
    .all-sections {
        margin-top: 40px;
        width: 100%;
    }

    .all-lists {
        list-style: none;
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: center;
        gap: 15px;
        align-items: center;
    }
    .all-lists li {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        align-items: center;
        border: 3px solid rgba(59, 56, 202, 0.1);
        padding: 10px 20px;
        border-radius: 12px;
        width: 100%;
        max-width: 350px;
        text-align: left;
    }

    .all-lists li:hover {
        background: rgba(46, 49, 247, 0.1);
    }

    .all-lists img{
        width: 50px;
        height: 50px;
        border-radius: 50%;
        margin-right: 15px;
        object-fit: cover;
    }
    .feature-thingyyy {
        display: flex;
        align-items: center;
        font-size: 1.1rem;
        font-weight: 500; 
        margin-bottom: 10px;
    }
</style>