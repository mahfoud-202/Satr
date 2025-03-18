<script>
    import TopBar from "./components/TopBar.svelte";
    import Workspace from "./components/Workspace.svelte";
    import StatusBar from "./components/StatusBar.svelte";
</script>

<div class="app">
    <TopBar />
    <Workspace />
    <StatusBar />
</div>

<style>
    .app {
        display: grid;
        grid-template-rows: 40px minmax(0, 1fr) 40px;
        width: 100%;
        height: 100%;
        overflow: hidden;
    }
</style>
