<div class="footer">
    <div class="footer__top">
        <div class="links">
            <h3>Links</h3>
            <ul>
                <li>
                    <a href="/about">Home</a>
                </li>
                <li>
                    <a href="/stack">Stack</a>
                </li>
                <li>
                    <a href="/workspace">Workspace</a>
                </li>
                <li>
                    <a href="/works">Works</a>
                </li>
            </ul>
        </div>
        <div class="elsewhere">
            <h3>Elsewhere</h3>
            <ul>
                <li>
                    <a href="https://t.me/icykit" target="_blank">Telegram</a>
                </li>
                <li>
                    <a href="https://github.com/IcyKit" target="_blank">GitHub</a>
                </li>
                <li>
                    <a href="https://discord.com/users/193069352554201088/" target="_blank">Discord</a>
                </li>
                <li>
                    <a href="https://www.linkedin.com/in/nikita-efimov-756461237/" target="_blank">LinkedIn</a
                    >
                </li>
            </ul>
        </div>
    </div>
    <p>© 2023 Nikita Efimov. All Rights Reserved.</p>
</div>

<style>
    .footer {
        padding-top: 50px;
        padding-bottom: 20px;
    }

    .footer__top {
        display: grid;
        grid-template-columns: 1fr 1fr;
        margin-bottom: 50px;
    }

    h3 {
        font-size: 14px;
        font-weight: bold;
        margin-bottom: 20px;
    }

    ul {
        display: flex;
        flex-direction: column;
        gap: 12px;
    }

    a {
        font-size: 14px;
    }

    a:hover {
        color: rgb(102, 102, 102);
    }

    p {
        color: #aaaaaa;
        font-size: 14px;
    }

    @media (max-width: 425px) {
        .footer {
            padding-top: 30px;
        }

        .footer__top {
            margin-bottom: 40px;
            justify-items: center;
        }

        h3 {
            margin-bottom: 20px;
        }

        p {
            text-align: center;
        }

        h3,
        li,
        a,
        p {
            font-size: 12px;
        }
    }
</style>
