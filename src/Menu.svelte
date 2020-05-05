
<script>
    import Toggle from './Toggle.svelte';

    let src = 'https://media.giphy.com/media/jOgRWnCyyRqLaCjHMS/source.gif';

</script>

<Toggle title="Toggle Header" isActive={true}>
    <div class="content">
        <img {src} alt="test" id="imageTest"/>
    </div>
</Toggle>
<br/><br/>

