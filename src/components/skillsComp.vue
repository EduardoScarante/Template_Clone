<script>

export default {
    props: {
        path: String,
        title: String,
        subtitle: String
    }

}

</script>


<template>
    <section>
        <main id="content">
            <img :src="path" alt="">
            <p>{{ title }}</p>
            <p class="sub">{{ subtitle }}</p>
        </main>
    </section>
</template>


<style scoped>
section {
    display: flex;
    justify-content: center;

    margin-top: 100px;
    margin-bottom: 100px;
}

#content {
    height: 450px;
    width: 250px;
    color: black;

    display: flex;
    justify-content: space-around;
    flex-direction: column;
    align-items: center;
    text-align: center;
}

#content img {
    width: 150px;
    height: 150px;
}

#content p {
    font-weight: 600;
    font-size: 1.5rem;
}

#content .sub {
    font-weight: 400;
    font-size: 1rem;
}

@media (max-width: 600px) {
    section {

        margin-top: 10px;
        margin-bottom: 10px;
    }
}
</style>