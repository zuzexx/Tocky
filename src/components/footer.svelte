<script>
</script>

<footer>
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
        <img src="images/facebook-logo.png" alt="" class="facebook">
        <img src="images/tik-tok.png" alt="" class="tiktok">
        <img src="images/instagram-logo.png" alt="" class="instagram">
        <img src="images/twitter-logo.png" alt="" class="twitter">
    </div>
</footer>
 <style>
    footer{
        width: 80vw;
        height: auto;
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
    }
    ul{
        list-style-type: none;
        text-align: left;
    }

    @media only screen and (min-width: 1200px) {
        
        .footer-container{
            width: 50vw;
            display: flex;
            flex-direction: row;
            justify-content: space-between;
            align-items: center;
        }
        hr{
            display: none;
        }
    }
 </style>
