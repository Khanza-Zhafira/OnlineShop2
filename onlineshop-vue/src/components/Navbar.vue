<template>
    <nav class="navbar-wrap">
        <div class="judul">
            <p class="brand">
                <b>SMK YADIKA SOREANG - ONLINESHOP</b>
            </p>

            <div class="nav-links">
                <RouterLink to="/">Landing</RouterLink>
                <RouterLink to="/about">About</RouterLink>
                <RouterLink to="/product">Product</RouterLink>
                <RouterLink to="/contact">Contact</RouterLink>
            </div>
        </div>
    </nav>
</template>

<style scoped>
.navbar-wrap {
    width: min(1200px, calc(100% - 32px));
    margin: 20px auto 0;
}

.judul {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 20px;
    background: rgba(255, 255, 255, 0.9);
    border: 1px solid #e6edf9;
    border-radius: 18px;
    padding: 18px 24px;
    box-shadow: 0 10px 24px rgba(15, 23, 42, 0.05);
}

.brand {
    margin: 0;
    font-size: 0.96rem;
    color: #1f4ca8;
}

.nav-links {
    display: flex;
    align-items: center;
    gap: 18px;
    flex-wrap: wrap;
}

.nav-links a {
    padding: 8px 12px;
    border-radius: 10px;
    color: #475569;
    font-weight: 600;
    transition: all 0.2s ease;
}

.nav-links a:hover,
.nav-links a.router-link-active {
    background: #eaf3ff;
    color: #1d4ed8;
}

@media (max-width: 640px) {
    .judul {
        flex-direction: column;
        text-align: center;
    }

    .brand {
        font-size: 0.82rem;
    }

    .nav-links {
        justify-content: center;
    }
}
</style>
     