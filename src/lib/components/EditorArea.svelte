<script>
    import VerticalSpliter from "./VerticalSpliter.svelte";
    import View from "./View.svelte";
    import SideBar from "./SideBar.svelte";

    const SIZE = 256;

    let showRegionA = $state(false);
    let x = $state(SIZE);
    let l = $state("<");

    $effect(() => {
        if (showRegionA) {
            x = 0;
            l = ">";
        } else {
            x = SIZE;
            l = "<";
        }
    });

    function toggle() {
        showRegionA = !showRegionA;
    }
</script>

<div class="editor-area" style="grid-template-columns: {x}px 20px minmax(0, 1fr);">
    <SideBar />
    <VerticalSpliter label={l} onClickHandler={toggle}/>
    <View />
</div>

<style>
    .editor-area {
        display: grid;
        border: 1px solid white;
        min-width: 0px;
        min-height: 0px;
        width: 100%;
        height: 100%;
        overflow: hidden;
    }
</style>
