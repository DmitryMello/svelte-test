<nav>
    <div class="nav-cotainer">
        <a href ="/" class="nav-logo" title="back to Hoepage">Николаев Дмитрий</a>
    <div class="nav=links">
        {#if nav as link.isShow}

        <a href={link.href} class="link">{link.title}</a>
        
        {/if}
        </div>
    </div>
</nav>
<div class="container">
    <!--Pages will be injected below-->
    <slot></slot>
</div>
<script>
    const nav = [
    {
    title: "обо мне",
    href: "/about",
    isShow: true,
    },
    {
    title: "Блог",
    href: "/blog",
    isShow: true,
    },
    {
    title: "Портфолио",
    href: "/project",
    isShow: true,
    },
    {
    title: "Контакты",
    href: "/contact",
    isShow: true,
    },
    {
    title:"temp",
    href:"/temp",
    isShow: false,
}
    ]
    </script>

    <style>
        .container{
            max-width: 1400px;
            margin: 50px auto;
        }
    </style>
