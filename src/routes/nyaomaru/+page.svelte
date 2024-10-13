<script lang="ts">
import NyaomaruButton from "./NyaomaruButton.svelte";

let count = 0;

const countUp = () => {
	count += 1;
};

const countDown = () => {
	count -= 1;
};

const countUpButtonLabel = "count up";
const countDownButtonLabel = "count down";
</script>

<svelte:head>
	<title>Nyaomaru</title>
	<meta name="description" content="Nyaomaru page" />
</svelte:head>

<sections class="nyaomaru">
    <h1>nyaomaru</h1>
    <p>nyaomaru page</p>
    <div class="buttonArea">
        <NyaomaruButton fn={countUp} label={countUpButtonLabel}/>
        <NyaomaruButton fn={countDown} label={countDownButtonLabel}/>
    </div>
    <div class="countArea">
        <p>count: {count}</p>
    </div>
</sections>

<style>
    .nyaomaru {
        color: black;

    }
    .buttonArea {
        display: flex;
        justify-content: center;
        gap: 16px;
    }
    .countArea {
        display: flex;
        justify-content: center;
    }
</style>
