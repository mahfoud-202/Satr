<script>
    import ActivityBar from "./ActivityBar.svelte";
    import EditorArea from "./EditorArea.svelte";
</script>

<div class="workspace">
    <ActivityBar />
    <EditorArea />
</div>

<style>
    .workspace {
        display: grid;
        grid-template-columns: 40px minmax(0, 1fr);
        border: 1px solid white;
        min-width: 0px;
        min-height: 0px;
        width: 100%;
        height: 100%;
    }
</style>
