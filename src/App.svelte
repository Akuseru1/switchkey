<script>
    import css from "./main.css";

    import Header from "./components/header.svelte";
    import Footer from "./components/footer.svelte";

    import Router from "svelte-spa-router";
    import routes from "./routes.js";
</script>

<main>
    <Header />
    <Router {routes} />
    <Footer />
</main>

<style>
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
    :root {
        font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
            Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
    }

    main {
        text-align: center;
        margin: 0 auto;
    }

    img {
        height: 16rem;
        width: 16rem;
    }

    h1 {
        color: #ff3e00;
        text-transform: uppercase;
        font-size: 4rem;
        font-weight: 100;
        /* line-height: 1.1;
        margin: 2rem auto;
        max-width: 14rem; */
    }

    p {
        /* max-width: 14rem;
        margin: 1rem auto;
        line-height: 1.35; */
    }

    /* @media (min-width: 480px) {
        h1 {
            max-width: none;
        }

        p {
            max-width: none;
        }
    } */
</style>
