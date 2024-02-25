<script>
    let videoSrc = 'src/assets/videos/andromeda_galaxy.mp4'
    let slogan = 'TO INFINITY AND BEYOND'

    function handleClick(event) {
        event.preventDefault()
        event.target.blur()
    }
</script>

<div class="wrapper">
    <input type="checkbox" on:click={handleClick}>
    <div class="video">
        <video src={videoSrc} loop muted autoplay playsinline></video>
    </div>
    <div class="text">
        <span data-text={slogan}></span>
    </div>
</div>

<style>
    @import '../../style/welcome-button.scss';
</style>
  
  