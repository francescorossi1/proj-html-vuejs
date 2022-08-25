<template>
    <div class="wrapper my-5">
        <div class="content text-center text-white py-lg">
            <p><i class="fa-solid fa-quote-left fa-3x tc-lime py-5"></i></p>
            <p class="font-size-24 mb-5">
                {{person.quote}}
            </p>
            <figure>
                <img :src="require(`../assets/img/${person.photoSrc}`)" :alt="person.name" class="img-fluid mt-5">
                <figcaption>
                    <h5 class="pt-3 tc-lime">{{person.name}}</h5>
                    <span>{{person.role}}</span>
                </figcaption>
            </figure>
        </div>
    </div>
</template>

<script>
export default {
    name: 'QuotesSection',
    data () {
        return {
            person: { name: 'Lissa Durbin', role: 'Client', photoSrc: 'objectives-1.jpg', quote: 'When it comes to barbequing, there are two main schools of thought for the techniques that you can use.\
                Freshly scrambled eggs with applewood smoked bacon - are amazing!'}
        }
    }
}
</script>

<style lang="scss" scoped>
.wrapper {
    background-image: url('../assets/img/quotes-1.jpg');
    background-size: cover;
    background-position: center;
}

.content {
    background-color: rgba(0, 0, 0, 0.6);

    p {
        max-width: 60%;
        margin: 0 auto;
    }

    img {
        width: 7vw;
        height: 7vw;
        border-radius: 50%;
        border: 2px solid white;
    }
}
</style>