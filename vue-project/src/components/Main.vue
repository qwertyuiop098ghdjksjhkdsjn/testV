<script setup>

</script>

<template>
 
 <modal-window ref="modal"></modal-window>
    <header>
        <div class="container">
            <div class="main">
                <img src="./images/logo 1.png"/>
                <div class="menu">
                    <h6>Games</h6>
                    <h6>Contact Us</h6>
                    <h6>Terms of Use</h6>
                    <h6>About</h6>
                </div>
            </div>
            <div class="buttons">
              <button class="signUp" @click="showModal">Sign up</button>
              <button class="logIn">Log in</button>                     
            </div>
        </div>
    </header>
    <section class="one">
        <h1>awesome html5 games - NO MONEY!</h1>
        <h3>Your Perfect Place To Get Some Fun And Excitement</h3>
        <div class="buttons_sectionOne">
            <button class="logIn_sectionOne">Log in</button>
            <button class="play">Play</button>            
        </div>
        <div class="form">
            <div class="form_sectionOne">
                <h2>Create a free account now</h2>
                <div class="form_container">
                    <div class="form_container_items">
                        <img src="./images//AboutUs_Dice_75x75__1_ 3.png"/> 
                        <p>1000+ Games available</p>   
                    </div>
                    <div class="form_container_items">
                        <img src="./images/AboutUs_Dice_75x75__1_ 1.png"/> 
                        <p>New game
                        Every week</p>
                    </div>
                    <div class="form_container_items">
                        <img src="./images/AboutUs_Dice_75x75__1_ 2.png"/> 
                        <p>Support our users 24/7</p>
                    </div>
                </div>
            </div>
            <div class="form_sectionOne_inputs">
                <input placeholder="Firstname"/>
                <input placeholder="Lastname"/>
                <input placeholder="Email address"/>
                <button>Join now</button>
            </div>
            <div class="form_sectionOne_checkbox">
                <input type="checkbox"/>
                <p>I accept the <span class="privacyPolicy">Privacy Policy</span></p>
            </div>
        </div> 
        <div class="headline">
            <div>
                <h4>Our Games</h4>
            <p>Get Virtual Welcome bonus after Sign Up</p>
            </div>
            <p>All games</p>
        </div>
    </section>
    <section class="two">
        <div class="cards">
            <div class="sixSmallCards">
                <div>
                    <img src="./images//gametype 1.png"/>
                    <p>Double Jackpot</p>
                    <p class="light">NetentGames</p>
                </div>

                <div>
                    <img src="./images//gametype 2.png"/>
                    <p>All Aboard: Dynam...</p>
                    <p class="light">RushGameStudio</p>
                </div>

                <div>
                    <img src="./images//gametype 3.png"/>
                    <p>Book Of Tombs</p>
                    <p class="light">NetentGames</p>
                </div>

                <div>
                    <img src="./images//gametype 5.png"/>
                    <p>Rudolph’s Ride</p>
                    <p class="light">NetentGames</p>
                </div>

                <div>
                    <img src="./images//gametype 6.png"/>
                    <p>Starburst XXXtreme</p>
                    <p class="light">StarBurst Inc.</p>
                </div>

                <div>
                    <img src="./images/gametype 8.png"/>
                    <p>Black Diamond</p>
                    <p class="light">RushGameStudio</p>
                </div>
            </div>
            <div class="threeBigCards">

                <div class="firstCard">
                    <div class="textContainer">
                       <div class="titleCard">Dynamite Riches
                        Megaways</div>
                    <div class="descriptionCard">Miners revealed a gain of €46,672 for Sandra M.! 
                        You too, dynamite the reels of the Red Tiger Daily Jackpot machines</div>
                    <button class="buttonCardPlay">Play now</button> 
                    </div>
                    <img src="./images/DynamiteRichesMW_BigWin_385x190 1.png"/>
                </div>

                <div class="secondCard">
                    <div class="textContainer">
                       <div class="titleCard">Gator Gold Deluxe Gigablox</div>
                    <div class="descriptionCard">These swamps conceal many dangers but especially precious treasures. 
                        Will you be able to find them?</div>
                    <button class="buttonCardPlay">Play now</button> 
                    </div>
                    <img src="./images/GOTM_GatorGold_385x190 1.png"/>
                </div>

                <div class="thirdCard">
                    <img src="./images/HomepageBanners_780x200_Promos 1.png"/>
                    <div class="thirdCardContainer">
                        <div class="thirdCardText">
                            <p>Our deals are not to be missed</p>
                            <p class="light">Discover a wide range of weekly promotions</p>
                        </div>
                        <button class="buttonCardMore">Read more</button>
                    </div>
                </div>

            </div>
            <div class="cardsText">* We don't offer opportunities to play for real money. Our games are free demo. 
                All games were invented for entertainment purposes only and do not offer real money prizes.</div>
        </div>
        
        <div class="form_sectionTwo">
            <div>
                <h1>Contact Us</h1>
            <p>If you have some questions, send us a message</p>
            </div>
            <div class="contactsContainer">
                <div class="form_sectionTwo_inputs">
                    <input placeholder="Firstname"/>
                    <input placeholder="Email address"/>
                    <textarea class="inputLarge" placeholder="Your message here..."></textarea>
                </div>
                <div class="form_sectionTwo_checkbox">
                    <div>
                        <input type="checkbox"/>
                        <p>I Accept The <span class="privacyPolicy">Privacy Policy</span></p>
                    </div> 
                    <button>Send</button>
                </div>
            </div>
        </div>
    </section>
    <footer>
        <div>
            <a>Disclaimer  |  Privacy Policy  |  Terms of Conditions</a>
        </div>
        <p class="paragraph">This site does not provide any form of online gambling and delivers information for entertainment and research purposes only. The games listed by Topwinningslots are intended for adult audience entertainment (underage visitors are restricted) and do not offer real money or prizes. 
            Practicing online free games does not imply future success at 'real money' gambling.
        </p>
        <div class="info">
            <p>2022 | © Lorem Inc. All Rights Reserved</p> 
            <div class="icons">
                <img src="./images/fa-brands_twitter.png"/>
                <img src="./images/fa-brands_facebook-f.png"/>
                <img src="./images/fa6-brands_instagram.png"/>
            </div>  
        </div>

    </footer>  
</template>

<script>
    import ModalWindow from './modal-window.vue'
 
    export default {
        name: 'Main',
        components: {
            ModalWindow
        },
        methods: {
            showModal: function () {
                this.$refs.modal.show = true
            }
        },
    }
</script>

<style lang="scss">
@import './styles.scss';
</style>
