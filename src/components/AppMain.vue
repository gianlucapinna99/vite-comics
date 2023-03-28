<script>
export default {
    data() {
        return {
            comics: [
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
            ]
        }
    },
    computed: {
        chunks() {
            const size = 5;
            return this.comics.reduce((chunks, item, i) => {
                if (i % size === 0) {
                    chunks.push([]);
                }
                chunks[chunks.length - 1].push(item);
                return chunks;
            }, []);
        }
    }
}
</script>

<template>
    <div class="jumbo"><img src="../assets/img/jumbotron.jpg" alt=""></div>
    <div class="container-bg">
        <button class="series">CURRENT SERIES</button>
        <div class="container">
            <div v-for="(chunk, index) in chunks" :key="index" class="row">
                <div v-for="item in chunk" :key="item.series" class="col-lg">
                    <div class="text-center">
                        <img :src="item.thumb" alt="thumbnail">
                        <p>{{ item.series }}</p>
                    </div>
                </div>
            </div>
        </div>
        <button class="load">LOAD MORE</button>
    </div>
</template>
  
<style>
.jumbo {
    height: 400px;
    overflow: hidden;
}


.container-bg {
    background-color: #1c1d1d;
    padding-top: 60px;
    padding-bottom: 40px;
}

p {
    color: white;
}

.container {
    width: 70%;
    margin: 0 auto;
}

.row {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}


.col-lg {
    flex-basis: calc(20% - 1rem);
    margin-right: 0.5rem;
    margin-left: 0.5rem;
}

.load {
    background-color: #0282f9;
    color: white;
    padding: 10px 60px;
    border: none;
    margin: 40px auto 40px auto;
    display: block;
}

.series {
    background-color: #0282f9;
    color: white;
    padding: 10px 30px;
    font-size: 25px;
    border: none;
    position: relative;
    top: -90px;
    left: 240px;
}
</style>
  