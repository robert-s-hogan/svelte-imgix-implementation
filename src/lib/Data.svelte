<script>
    export let url;
    export let classes;
</script>

<img
    srcset="{url}?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
        {url}?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
        {url}?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
        {url}?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
        {url}?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
        {url}?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
    src="{url}?auto=compress,format,enhance&fit=crop&w=320 640w"
    sizes="50vw"
    class={classes}
    alt="winery landscape"
>