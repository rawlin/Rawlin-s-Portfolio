<script>
    import '../global.css'
    import Redirect from '../components/RedirectComponent.svelte'
    import SeeMore from '../components/SeeMoreComponent.svelte'
</script>

<div class="container">
    <p>Hey, I'm Rawlin. I specialize in crafting user interfaces, interactions, and animations for mobile and web applications.</p>
    <div class="container-reactions">
        <Redirect redirectName="LinkedIn" redirectLink="https://www.linkedin.com/in/rawlin-crasto/" />
        <Redirect redirectName="Github" redirectLink="https://github.com/rawlin" />
    </div>
    <SeeMore class="see`"/>
</div>


<style>
    p {
        margin-bottom: 2em;
    }
    .container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 100vh;
    }
    .container-reactions {
        display: flex;
        justify-content: start;
        align-items: start;
    }
    .info-container {
        display: flex;
        flex-direction: column;
        justify-content: top;
        align-items: start;
        height: 100vh;
    }
    .see {
        position: absolute;
        bottom: 0;
        left: 50%;
        transform: translateX(-50%);
    }
    
</style>
