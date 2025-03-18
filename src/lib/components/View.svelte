<script></script>

<div class=panel>
    <div class="tabs">tabs</div>
    <div class="container"></div>
</div>

<style>
    .panel {
        display: grid;
        grid-template-rows: 40px minmax(0, 1fr);
    }
    .container {
        background-color: rgb(45, 50, 54);
        width: 100%;
        height: 100%;
        padding: 40px;
        overflow-y: scroll;
    }
    .tabs {
        display: flex;
        align-items: center;
        justify-content: center;
        background-color: rgb(32, 34, 48);
    }
</style>
