<template>
    <section>
    <header class="header-area transparent-bar section-padding-1">
        <div class="container-fluid">
            <div class="header-large-device">
                <div class="header-top header-top-ptb-1 border-bottom-1">
                    <div class="row">
                        <div class="col-xl-4 col-lg-5">

                        </div>
                        <div class="col-xl-8 col-lg-7">
                            <div class="header-top-right">
                                <div class="same-style-wrap">
                                    <div class="same-style same-style-border track-order">
                                        <a href="order-tracking.html">Track Your Order</a>
                                    </div>
                                    <div class="same-style same-style-border language-wrap">
                                        <a class="language-dropdown-active" href="#">English <i class="icon-arrow-down"></i></a>
                                        <div class="language-dropdown">
                                            <ul>
                                                <li><a href="#">English</a></li>

                                            </ul>
                                        </div>
                                    </div>
                                    <div class="same-style same-style-border currency-wrap">
                                        <a class="currency-dropdown-active" href="#">EGP Pound <i class="icon-arrow-down"></i></a>
                                        <div class="currency-dropdown">
                                            <ul>
                                                <li><a href="#">EGP</a></li>

                                            </ul>
                                        </div>
                                    </div>
                                </div>
                                <div class="social-style-1 social-style-1-mrg">
                                    <a href="#"><i class="icon-social-twitter"></i></a>
                                    <a href="#"><i class="icon-social-facebook"></i></a>
                                    <a href="#"><i class="icon-social-instagram"></i></a>
                                    <a href="#"><i class="icon-social-youtube"></i></a>
                                    <a href="#"><i class="icon-social-pinterest"></i></a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="header-bottom">
                    <div class="row align-items-center">
                        <div class="col-xl-2 col-lg-2">
                            <div class="logo">
                                <a href="index.html"><img src="assets/images/logo/logo.png" alt="logo"></a>
                            </div>
                        </div>
                        <div class="col-xl-8 col-lg-7">
                            <div class="main-menu main-menu-padding-1 main-menu-lh-1">
                                <nav>
                                    <ul>
                                        <li><a href="/">HOME </a>

                                        </li>
                                        <li><a href="shop.html">SHOP </a>
                                            <ul class="mega-menu-style mega-menu-mrg-1">
                                                <li>
                                                    <ul>
                                                        <li>
                                                            <a class="dropdown-title" href="#">Shop Categories</a>
                                                            <ul>
                                                                <li v-for="cat in categoris"  :key="cat.name" @mouseover="changeChild(cat)"><a href="index.html"> {{cat.name}}</a></li>

                                                            </ul>
                                                        </li>
                                                        <li>
                                                            <a class="dropdown-title" href="#">Category Type</a>
                                                            <ul>
                                                                <li v-for="child in catChild" :key="child.name"><a href="index.html"> {{child.name}}</a></li>

                                                            </ul>
                                                        </li>
                                                        <li>
                                                            <a href="shop.html"><img src="assets/images/banner/banner-12.png" alt=""></a>
                                                        </li>
                                                    </ul>
                                                </li>
                                            </ul>
                                        </li>
                                        <li><a href="#">DOWNLOAD </a>
                                            <ul class="sub-menu-style">
                                                <li><a href="about-us.html">about us </a></li>
                                                <li><a href="cart.html">cart page</a></li>
                                                <li><a href="checkout.html">checkout </a></li>
                                                <li><a href="my-account.html">my account</a></li>
                                                <li><a href="wishlist.html">wishlist </a></li>
                                                <li><a href="compare.html">compare </a></li>
                                                <li><a href="contact.html">contact us </a></li>
                                                <li><a href="order-tracking.html">order tracking</a></li>
                                                <li><a href="login-register.html">login / register </a></li>
                                            </ul>
                                        </li>
                                        <li><a href="blog.html">ABOUT US </a>
                                            <ul class="sub-menu-style">
                                                <li><a href="blog.html">blog standard </a></li>
                                                <li><a href="blog-no-sidebar.html">blog no sidebar </a></li>
                                                <li><a href="blog-right-sidebar.html">blog right sidebar</a></li>
                                                <li><a href="blog-details.html">blog details</a></li>
                                            </ul>
                                        </li>
                                        <li><a href="contact.html">CONTACT </a></li>
                                    </ul>
                                </nav>
                            </div>
                        </div>
                        <div class="col-xl-2 col-lg-3">
                            <div class="header-action header-action-flex header-action-mrg-right">
                                <div class="same-style-2 header-search-1">
                                    <a class="search-toggle" href="#">
                                        <i class="icon-magnifier s-open"></i>
                                        <i class="icon_close s-close"></i>
                                    </a>
                                    <div class="search-wrap-1">
                                        <form action="#">
                                            <input placeholder="Search products…" type="text">
                                            <button class="button-search"><i class="icon-magnifier"></i></button>
                                        </form>
                                    </div>
                                </div>
                                <div class="same-style-2">
                                    <a href="login-register.html"><i class="icon-user"></i></a>
                                </div>
                                <div class="same-style-2">
                                    <a href="wishlist.html"><i class="icon-heart"></i><span class="pro-count red">03</span></a>
                                </div>
                                <div class="same-style-2 header-cart">
                                    <a class="cart-active" href="#">
                                        <i class="icon-basket-loaded"></i><span class="pro-count red">02</span>
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="header-small-device small-device-ptb-1">
                <div class="row align-items-center">
                    <div class="col-5">
                        <div class="mobile-logo">
                            <a href="index.html">
                                <img alt="" src="assets/images/logo/logo.png">
                            </a>
                        </div>
                    </div>
                    <div class="col-7">
                        <div class="header-action header-action-flex">
                            <div class="same-style-2">
                                <a href="login-register.html"><i class="icon-user"></i></a>
                            </div>
                            <div class="same-style-2">
                                <a href="wishlist.html"><i class="icon-heart"></i><span class="pro-count red">03</span></a>
                            </div>
                            <div class="same-style-2 header-cart">
                                <a class="cart-active" href="#">
                                    <i class="icon-basket-loaded"></i><span class="pro-count red">02</span>
                                </a>
                            </div>
                            <div class="same-style-2 main-menu-icon">
                                <a class="mobile-header-button-active" href="#"><i class="icon-menu"></i> </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </header>
    <!-- mini cart start -->
    <div class="sidebar-cart-active">
        <div class="sidebar-cart-all">
            <a class="cart-close" href="#"><i class="icon_close"></i></a>
            <div class="cart-content">
                <h3>Shopping Cart</h3>
                <ul>
                    <li class="single-product-cart">
                        <div class="cart-img">
                            <a href="#"><img src="assets/images/cart/cart-1.jpg" alt=""></a>
                        </div>
                        <div class="cart-title">
                            <h4><a href="#">Simple Black T-Shirt</a></h4>
                            <span> 1 × $49.00	</span>
                        </div>
                        <div class="cart-delete">
                            <a href="#">×</a>
                        </div>
                    </li>
                    <li class="single-product-cart">
                        <div class="cart-img">
                            <a href="#"><img src="assets/images/cart/cart-2.jpg" alt=""></a>
                        </div>
                        <div class="cart-title">
                            <h4><a href="#">Norda Backpack</a></h4>
                            <span> 1 × $49.00	</span>
                        </div>
                        <div class="cart-delete">
                            <a href="#">×</a>
                        </div>
                    </li>
                </ul>
                <div class="cart-total">
                    <h4>Subtotal: <span>$170.00</span></h4>
                </div>
                <div class="cart-checkout-btn">
                    <a class="btn-hover cart-btn-style" href="cart.html">view cart</a>
                    <a class="no-mrg btn-hover cart-btn-style" href="checkout.html">checkout</a>
                </div>
            </div>
        </div>
    </div>
    <!-- Mobile menu start -->
    <div class="mobile-header-active mobile-header-wrapper-style">
        <div class="clickalbe-sidebar-wrap">
            <a class="sidebar-close"><i class="icon_close"></i></a>
            <div class="mobile-header-content-area">
                <div class="header-offer-wrap mobile-header-padding-border-4">
                    <p><i class="icon-paper-plane"></i> FREE SHIPPING world wide for all orders over <span>$199</span></p>
                </div>
                <div class="mobile-search mobile-header-padding-border-1">
                    <form class="search-form" action="#">
                        <input type="text" placeholder="Search here…">
                        <button class="button-search"><i class="icon-magnifier"></i></button>
                    </form>
                </div>
                <div class="mobile-menu-wrap mobile-header-padding-border-2">
                    <!-- mobile menu start -->
                    <nav>
                        <ul class="mobile-menu">
                            <li class="menu-item-has-children"><a href="index.html">Home</a>
                                <ul class="dropdown">
                                    <li><a href="index.html">Home version 1 </a></li>
                                    <li><a href="index-2.html">Home version 2</a></li>
                                    <li><a href="index-3.html">Home version 3</a></li>
                                    <li><a href="index-4.html">Home version 4</a></li>
                                    <li><a href="index-5.html">Home version 5</a></li>
                                    <li><a href="index-6.html">Home version 6</a></li>
                                    <li><a href="index-7.html">Home version 7</a></li>
                                    <li><a href="index-8.html">Home version 8</a></li>
                                    <li><a href="index-9.html">Home version 9</a></li>
                                    <li><a href="index-10.html">Home version 10</a></li>
                                </ul>
                            </li>
                            <li class="menu-item-has-children "><a href="#">shop</a>
                                <ul class="dropdown">
                                    <li class="menu-item-has-children"><a href="#">shop layout</a>
                                        <ul class="dropdown">
                                            <li><a href="shop.html">standard style</a></li>
                                            <li><a href="shop-list.html">shop list style</a></li>
                                            <li><a href="shop-fullwide.html">shop fullwide</a></li>
                                            <li><a href="shop-no-sidebar.html">grid no sidebar</a></li>
                                            <li><a href="shop-list-no-sidebar.html">list no sidebar</a></li>
                                            <li><a href="shop-right-sidebar.html">shop right sidebar</a></li>
                                            <li><a href="store-location.html">store location</a></li>
                                        </ul>
                                    </li>
                                    <li class="menu-item-has-children"><a href="#">Products Layout</a>
                                        <ul class="dropdown">
                                            <li><a href="product-details.html">tab style 1</a></li>
                                            <li><a href="product-details-2.html">tab style 2</a></li>
                                            <li><a href="product-details-sticky.html">sticky style</a></li>
                                            <li><a href="product-details-gallery.html">gallery style </a></li>
                                            <li><a href="product-details-affiliate.html">affiliate style</a></li>
                                            <li><a href="product-details-group.html">group style</a></li>
                                            <li><a href="product-details-fixed-img.html">fixed image style </a></li>
                                        </ul>
                                    </li>
                                </ul>
                            </li>
                            <li class="menu-item-has-children"><a href="#">Pages</a>
                                <ul class="dropdown">
                                    <li><a href="about-us.html">about us </a></li>
                                    <li><a href="cart.html">cart page</a></li>
                                    <li><a href="checkout.html">checkout </a></li>
                                    <li><a href="my-account.html">my account</a></li>
                                    <li><a href="wishlist.html">wishlist </a></li>
                                    <li><a href="compare.html">compare </a></li>
                                    <li><a href="contact.html">contact us </a></li>
                                    <li><a href="order-tracking.html">order tracking</a></li>
                                    <li><a href="login-register.html">login / register </a></li>
                                </ul>
                            </li>
                            <li class="menu-item-has-children "><a href="#">Blog</a>
                                <ul class="dropdown">
                                    <li><a href="blog.html">blog standard </a></li>
                                    <li><a href="blog-no-sidebar.html">blog no sidebar </a></li>
                                    <li><a href="blog-right-sidebar.html">blog right sidebar</a></li>
                                    <li><a href="blog-details.html">blog details</a></li>
                                </ul>
                            </li>
                            <li><a href="contact.html">Contact us</a></li>
                        </ul>
                    </nav>
                    <!-- mobile menu end -->
                </div>
                <div class="mobile-header-info-wrap mobile-header-padding-border-3">
                    <div class="single-mobile-header-info">
                        <a href="order-tracking.html"><i class="lastudioicon-pin-3-2"></i> Track Your Order </a>
                    </div>
                    <div class="single-mobile-header-info">
                        <a class="mobile-language-active" href="#">Language <span><i class="icon-arrow-down"></i></span></a>
                        <div class="lang-curr-dropdown lang-dropdown-active">
                            <ul>
                                <li><a href="#">English</a></li>
                                <li><a href="#">French</a></li>
                                <li><a href="#">German</a></li>
                                <li><a href="#">Spanish</a></li>
                            </ul>
                        </div>
                    </div>
                    <div class="single-mobile-header-info">
                        <a class="mobile-currency-active" href="#">Currency <span><i class="icon-arrow-down"></i></span></a>
                        <div class="lang-curr-dropdown curr-dropdown-active">
                            <ul>
                                <li><a href="#">USD</a></li>
                                <li><a href="#">EUR</a></li>
                                <li><a href="#">Real</a></li>
                                <li><a href="#">BDT</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="mobile-contact-info mobile-header-padding-border-4">
                    <ul>
                        <li><i class="icon-phone "></i> (+612) 2531 5600</li>
                        <li><i class="icon-envelope-open "></i> norda@domain.com</li>
                        <li><i class="icon-home"></i> PO Box 1622 Colins Street West Australia</li>
                    </ul>
                </div>
                <div class="mobile-social-icon">
                    <a class="facebook" href="#"><i class="icon-social-facebook"></i></a>
                    <a class="twitter" href="#"><i class="icon-social-twitter"></i></a>
                    <a class="pinterest" href="#"><i class="icon-social-pinterest"></i></a>
                    <a class="instagram" href="#"><i class="icon-social-instagram"></i></a>
                </div>
            </div>
        </div>
    </div>

    </section>
</template>

<script>
    import axios from "axios";
    export default {
        name: "AppHeader",
        data:function(){
            return{
                categoris:[],
                catChild:[]
            }
        },
        mounted() {
            const head = { lang: "en" };
            axios.post("https://www.homrz.com/homrz_test/api/getCategories", head)
                .then(response => this.categoris = response.data.data);
        },
        methods:{
            changeChild(cat){
                this.catChild = cat.childrend;
            }
        }

    }
</script>

<style scoped>

</style>