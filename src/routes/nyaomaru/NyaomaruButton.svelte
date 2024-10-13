<script lang="ts">
import Button, { Label } from "@smui/button";

export let label = "";
export let fn = () => {};
</script>

<div class="nyaomaruButton">
    <Button on:click={fn} variant="raised">
        <Label>{label}</Label>
    </Button>
</div>

<style>
</style>

