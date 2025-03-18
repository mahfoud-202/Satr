<script>
    let { label, onClickHandler } = $props();
</script>

<!-- svelte-ignore a11y_click_events_have_key_events -->
<!-- svelte-ignore a11y_no_static_element_interactions -->
<div class="v-resizer" onclick={onClickHandler}>
    { label }
</div>

<style>
    .v-resizer {
        display: flex;
        align-items: center;
        justify-content: center;
        background-color: #2d2f31;
        user-select: none;
        width: 100%;
        height: 100%;
    }
    .v-resizer:hover {
        cursor: pointer;
        background-color: aqua;
    }
    .v-resizer:active {
        background-color: aqua;
    }
</style>
