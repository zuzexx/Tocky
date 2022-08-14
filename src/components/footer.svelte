<script>
</script>

<footer>
    <hr>
    <div class="footer-container">

        <div class="solutions-container">
            <h5>Solutions</h5>
            <ul>
                <li>+1 234 567 8900</li>
                <li>+44 1234 123456</li>
                <li>support@tracky.com</li>
            </ul>
        </div>
        <div class="company-container">
            <h5>Company</h5>
            <ul>
                <li>About</li>
                <li>Blog</li>
                <li>Jobs</li>
            </ul>
        </div>
        <div class="support-container">
            <h5>Support</h5>
            <ul>
                <li>Pricing</li>
                <li>FAQs</li>
                <li>Contact</li>
            </ul>
        </div>
            <div class="legal-container">
                <h5>Legal</h5>
            <ul>
                <li>Terms</li>
                <li>Privacy</li>
                <li>Refunds</li>
            </ul>
            </div>
    
    </div>
    <hr>
    <div class="social-media">
        <a href="www.facebook.com"><img src="images/facebook-logo.png" alt="" class="facebook"></a>
        <a href="www.tiktok.com"><img src="images/tik-tok.png" alt="" class="tiktok"></a>
        <a href="www.instagram.com"><img src="images/instagram-logo.png" alt="" class="instagram"></a>
        <a href="www.twitter.com"><img src="images/twitter-logo.png" alt="" class="twitter"></a>
    </div>
</footer>
 <style>
    footer{
        width: 80vw;
        height: auto;
        margin-top: 6rem;
        padding:2rem;
       
    }
    li{
        font-size: 0.8rem;
        font-weight: var(--light);
        color:var(--button-hover) ;
        padding: 0.2rem;
    }
    li:hover{
        cursor:pointer;
        text-decoration: underline;
    }
    
    .footer-container{
        width: 80vw;
        display: gird;
        justify-content: center;
        align-items: center;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 1fr 1fr;
    }
    img{
        width: 40px;
    }
    hr{
        width: 80vw;
        margin: auto;
        margin-bottom: 2rem;
        margin-top: 2rem;
        border:none;
        height: 3px;
        background-color: var(--header);
        
    }
    ul{
        list-style-type: none;
        text-align: left;
    }

    @media only screen and (min-width: 1200px) {
        footer{
            width: 50vw;
        }
        .footer-container{
            width: 50vw;
            display: flex;
            flex-direction: row;
            justify-content: space-between;
            align-items: center;
        }
        hr{
            width: 50vw;
        }
        li{
            font-size: 0.9rem;
        }
       
    }
 </style>
