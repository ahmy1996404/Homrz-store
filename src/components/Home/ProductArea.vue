<template>
    <div class="product-area pb-80">
        <div class="container">
            <div class="section-title-2 text-center mb-45" style="margin-top: 15px">
                <h2><span>Best</span>Sells</h2>
                <p>Top our product best selling</p>
            </div>
            <div class="tab-btn-wrap mb-40">
                <div class="tab-style-2 nav">
                    <a class="active" href="#product-1" data-toggle="tab">Best Sells</a>

                </div>
                <div class="btn-style-2">
                    <a class="animated" href="shop.html">see all product <i class="icon-arrow-right"></i></a>
                </div>
            </div>
            <div class="tab-content jump">
                <div id="product-1" class="tab-pane active">
                    <div class="row">
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12" v-for="(product ,index) in products" :key="product.id">
                            <div class="single-product-wrap mb-35" v-if="index<12">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img v-if="product.images[0] != null" style="height: 324px" :src="product.images[0].images" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" @click="productModal(product)" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html" v-text="product.title"></a></h3>
                                    <div class="product-price-2">
                                        <span  v-text="product.price + ' EGP'"></span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html" v-text="product.title"></a></h3>
                                    <div class="product-price-2">
                                        <span  v-text="product.price + ' EGP'"></span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div id="product-2" class="tab-pane">
                    <div class="row">
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-20.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Snakeskin print belt</a></h3>
                                    <div class="product-price-2">
                                        <span>$20.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Snakeskin print belt</a></h3>
                                    <div class="product-price-2">
                                        <span>$20.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-19.jpg" alt="">
                                    </a>
                                    <span class="pro-badge left bg-red">-20%</span>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Faded Grey T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Faded Grey T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-18.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Tie-up Sute Sandals</a></h3>
                                    <div class="product-price-2">
                                        <span>$35.45</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Tie-up Sute Sandals</a></h3>
                                    <div class="product-price-2">
                                        <span>$35.45</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-17.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <h3><a href="product-details.html">Vintage Socks X3</a></h3>
                                    <div class="product-price-2">
                                        <span>$45.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <h3><a href="product-details.html">Vintage Socks X3</a></h3>
                                    <div class="product-price-2">
                                        <span>$45.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-16.jpg" alt="">
                                    </a>
                                    <span class="pro-badge left bg-red">-20%</span>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <h3><a href="product-details.html">Simple Rounded Sunglasses</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <h3><a href="product-details.html">Simple Rounded Sunglasses</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-15.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Basic White Simple Sneaker</a></h3>
                                    <div class="product-price-2">
                                        <span>$55.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Basic White Simple Sneaker</a></h3>
                                    <div class="product-price-2">
                                        <span>$55.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-14.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Make Thing Happen T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span>$65.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Make Thing Happen T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span>$65.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-13.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Basic Joggin Shorts</a></h3>
                                    <div class="product-price-2">
                                        <span>$75.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Basic Joggin Shorts</a></h3>
                                    <div class="product-price-2">
                                        <span>$75.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div id="product-3" class="tab-pane">
                    <div class="row">
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-16.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Simple Rounded Sunglasses</a></h3>
                                    <div class="product-price-2">
                                        <span>$20.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Simple Rounded Sunglasses</a></h3>
                                    <div class="product-price-2">
                                        <span>$20.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-15.jpg" alt="">
                                    </a>
                                    <span class="pro-badge left bg-red">-20%</span>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Basic White Simple Sneaker</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Basic White Simple Sneaker</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-14.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Make Thing Happen T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span>$35.45</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Make Thing Happen T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span>$35.45</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-13.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <h3><a href="product-details.html">Basic Joggin Shorts</a></h3>
                                    <div class="product-price-2">
                                        <span>$45.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <h3><a href="product-details.html">Basic Joggin Shorts</a></h3>
                                    <div class="product-price-2">
                                        <span>$45.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-20.jpg" alt="">
                                    </a>
                                    <span class="pro-badge left bg-red">-20%</span>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <h3><a href="product-details.html">Snakeskin print belt</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <h3><a href="product-details.html">Snakeskin print belt</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-19.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Faded Grey T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span>$55.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Faded Grey T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span>$55.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-18.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Tie-up Sute Sandals</a></h3>
                                    <div class="product-price-2">
                                        <span>$65.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Tie-up Sute Sandals</a></h3>
                                    <div class="product-price-2">
                                        <span>$65.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-17.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Vintage Socks X3</a></h3>
                                    <div class="product-price-2">
                                        <span>$75.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Vintage Socks X3</a></h3>
                                    <div class="product-price-2">
                                        <span>$75.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div id="product-4" class="tab-pane">
                    <div class="row">
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-14.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Make Thing Happen T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span>$20.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Make Thing Happen T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span>$20.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-13.jpg" alt="">
                                    </a>
                                    <span class="pro-badge left bg-red">-20%</span>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Basic Joggin Shorts</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Basic Joggin Shorts</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-16.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Simple Rounded Sunglasses</a></h3>
                                    <div class="product-price-2">
                                        <span>$35.45</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Simple Rounded Sunglasses</a></h3>
                                    <div class="product-price-2">
                                        <span>$35.45</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-15.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <h3><a href="product-details.html">Basic White Simple Sneaker</a></h3>
                                    <div class="product-price-2">
                                        <span>$45.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <h3><a href="product-details.html">Basic White Simple Sneaker</a></h3>
                                    <div class="product-price-2">
                                        <span>$45.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-18.jpg" alt="">
                                    </a>
                                    <span class="pro-badge left bg-red">-20%</span>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <h3><a href="product-details.html">Tie-up Sute Sandals</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <h3><a href="product-details.html">Tie-up Sute Sandals</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-17.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Vintage Socks X3</a></h3>
                                    <div class="product-price-2">
                                        <span>$55.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Vintage Socks X3</a></h3>
                                    <div class="product-price-2">
                                        <span>$55.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-20.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Snakeskin print belt</a></h3>
                                    <div class="product-price-2">
                                        <span>$65.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Snakeskin print belt</a></h3>
                                    <div class="product-price-2">
                                        <span>$65.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-19.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Faded Grey T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span>$75.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Faded Grey T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span>$75.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div id="product-5" class="tab-pane">
                    <div class="row">
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-15.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Basic White Simple Sneaker</a></h3>
                                    <div class="product-price-2">
                                        <span>$20.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Basic White Simple Sneaker</a></h3>
                                    <div class="product-price-2">
                                        <span>$20.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-13.jpg" alt="">
                                    </a>
                                    <span class="pro-badge left bg-red">-20%</span>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Basic Joggin Shorts</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Basic Joggin Shorts</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-16.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Simple Rounded Sunglasses</a></h3>
                                    <div class="product-price-2">
                                        <span>$35.45</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Simple Rounded Sunglasses</a></h3>
                                    <div class="product-price-2">
                                        <span>$35.45</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-14.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <h3><a href="product-details.html">Make Thing Happen T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span>$45.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <h3><a href="product-details.html">Make Thing Happen T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span>$45.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-19.jpg" alt="">
                                    </a>
                                    <span class="pro-badge left bg-red">-20%</span>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <h3><a href="product-details.html">Faded Grey T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <h3><a href="product-details.html">Faded Grey T-Shirt</a></h3>
                                    <div class="product-price-2">
                                        <span class="new-price">$35.45</span>
                                        <span class="old-price">$45.80</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-17.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Vintage Socks X3</a></h3>
                                    <div class="product-price-2">
                                        <span>$55.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Vintage Socks X3</a></h3>
                                    <div class="product-price-2">
                                        <span>$55.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-20.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Snakeskin print belt</a></h3>
                                    <div class="product-price-2">
                                        <span>$65.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Snakeskin print belt</a></h3>
                                    <div class="product-price-2">
                                        <span>$65.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 col-12">
                            <div class="single-product-wrap mb-35">
                                <div class="product-img product-img-zoom mb-15">
                                    <a href="product-details.html">
                                        <img src="assets/images/product/product-18.jpg" alt="">
                                    </a>
                                    <div class="product-action-2 tooltip-style-2">
                                        <button title="Wishlist"><i class="icon-heart"></i></button>
                                        <button title="Quick View" data-toggle="modal" data-target="#exampleModal"><i class="icon-size-fullscreen icons"></i></button>
                                        <button title="Compare"><i class="icon-refresh"></i></button>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Tie-up Sute Sandals</a></h3>
                                    <div class="product-price-2">
                                        <span>$75.50</span>
                                    </div>
                                </div>
                                <div class="product-content-wrap-2 product-content-position text-center">
                                    <div class="product-rating-wrap">
                                        <div class="product-rating">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star gray"></i>
                                        </div>
                                        <span>(2)</span>
                                    </div>
                                    <h3><a href="product-details.html">Tie-up Sute Sandals</a></h3>
                                    <div class="product-price-2">
                                        <span>$75.50</span>
                                    </div>
                                    <div class="pro-add-to-cart">
                                        <button title="Add to Cart">Add To Cart</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>

<script>
    export default {
        name: "ProductArea",
        props:['products'],
        data:function () {
            return{
               

            }

        },
        computed: {
            modalProduct: function () {
                // `this` points to the vm instance
                return  this.$store.state.modalProduct;
            }

        },
        methods:{
            productModal: function (Product) {
                // `this` points to the vm instance
                this.$store.state.modalProduct[0].title = Product.title ;
                this.$store.state.modalProduct[0].desc = Product.description ;
                this.$store.state.modalProduct[0].price = Product.price ;
                this.$store.state.modalProduct[0].color = Product.color ;
                this.$store.state.modalProduct[0].categories = Product.category ;
                this.$store.state.modalProduct[0].tags = Product.tags ;
                this.$store.state.modalProduct[0].images = Product.images ;
                this.$store.state.modalProduct[0].firstImg = Product.images[0].images ;


                console.log(this.$store.state.modalProduct[0].images);
            }
        }

    }
</script>

<style scoped>

</style>