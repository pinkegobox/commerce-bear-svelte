<script>
    export let ref;
    export let handleBarClick;
    export let handleModalClick;
</script>

<style>
.closeAnnoucement {
    position: absolute;
    top: 0;
    right: 0;
    display: flex;
    align-items: center;
    justify-content: center;
}

.closeAnnoucement:after {
    content: '×';
    display: block;
    font-family: helvetica,arial,sans-serif;
    font-weight: normal;
    cursor: pointer;
}
</style>

<span
    class="closeAnnoucement"
    tabIndex="0"
    role="button"
    aria-label="Close Announcement"
    {ref}
    on:click={handleBarClick}
    on:click={handleModalClick}
></span>