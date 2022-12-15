<div class="p-5 min-h-40">
    <div class="lg:w-3/5 lg:m-auto bg-stone-100 mx-2 px-5 py-10 text-center relative h-[12rem]">
        <p class="lg:w-1/3 text-sm lg:text-lg font-['Indie_Flower']">{data[index].name} says...</p>
        <div class="flex flex-row items-center relative justify-center">
            <button class="absolute border -left-8 lg:left-2" on:click={memeLeft}>
                <img src="/circle-chevron-left-solid.svg" width="25" height="25" alt="Review slider left icon"/>
            </button>
            <q class="text-md lg:text-xl h-20 font-['DM_Serif_Display']">{data[index].review}</q>
            <button class="absolute border -right-8 lg:right-2" on:click={memeRight}>
                <img src="/circle-chevron-right-solid.svg" width="25" height="25" alt="Review slider right icon"/>
            </button>
        </div>
    </div>
</div>

<script lang="ts">
        let index: number = 0;

        let data = [
        {
            id: 1,
            name: 'Lisa',
            review: 'Great haircut!!! Top notch customer service, would easily use again.'
        },
        {
            id: 2,
            name: 'Martin',
            review: "Wonderful hair stylist. Would highly recommend if you're looking for high quality hair treatments"
        }
    ]

    const memeLeft = () => {
        if (index == 0) {
            index = (data.length - 1);
        } else {
            index--;
        }
    }

    const memeRight = () => {
        if (index == (data.length - 1)) {
            index = 0;
        } else {
            index++;
        }
    }
</script>