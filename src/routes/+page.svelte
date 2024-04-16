<script>
    import '../global.css'
    import Redirect from '../components/RedirectComponent.svelte'
    import SeeMore from '../components/SeeMoreComponent.svelte'
</script>

<div class="main-container flex flex-col justify-center items-center min-h-screen">
    <p class="mb-5 p-7 text-start">Hey, I'm Rawlin. I specialize in crafting user interfaces, interactions and animations for mobile and web applications.</p>
    <div class="flex flex-row items-start justify-start space-x-7 text-sm">
        <Redirect redirectName="LinkedIn" redirectLink="https://www.linkedin.com/in/rawlin-crasto/" />
        <Redirect redirectName="Github" redirectLink="https://github.com/rawlin" />
    </div>
    <SeeMore class="see-more-component absolute bottom-6 left-1/2 transform -translate-x-1/2"/>
</div>
