<template>
    <div class="modal fade" id="exampleModal" tabindex="-1" role="dialog">
        <div class="modal-dialog" role="document">
            <div class="modal-content">
                <div class="modal-header">
                    <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">x</span></button>
                </div>
                <div class="modal-body">
                    <div class="row">
                        <div class="col-lg-5 col-md-6 col-12 col-sm-12">
                            <div class="tab-content quickview-big-img">
                                <div id="pro-1" class="tab-pane fade show active">
                                    <img style="height:440px" :src="photo" alt="">
                                </div>
                                <div  class="tab-pane fade">
                                    <img :src="photo" style="height: 90px" alt="">
                                </div>

                            </div>
                            <div class="quickview-wrap mt-15">
                                <div class=" nav-style-6">
<!--                                    <a class="active" data-toggle="tab" :href="'#'+modalProduct[0].images[0].id"><img style="height:90px" :src="modalProduct[0].images[0].images" alt=""></a>-->
                                    <a data-toggle="active tab" v-for="image in modalProduct[0].images" :key="image.images" ><img @click="photo=image.images" :src="image.images" style="height: 90px; width: 90px ; margin-right: 5px"  alt=""></a>

                                </div>
                            </div>
                        </div>
                        <div class="col-lg-7 col-md-6 col-12 col-sm-12">
                            <div class="product-details-content quickview-content">
                                <h2  v-text="modalProduct[0].title"></h2>
                                <div class="product-ratting-review-wrap">
                                    <div class="product-ratting-digit-wrap">
                                        <div class="product-ratting">
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                            <i class="icon_star"></i>
                                        </div>
                                        <div class="product-digit">
                                            <span>5.0</span>
                                        </div>
                                    </div>
                                    <div class="product-review-order">
                                        <span>62 Reviews</span>
                                        <span>242 orders</span>
                                    </div>
                                </div>
                                <p>{{modalProduct[0].desc}}</p>
                                <div class="pro-details-price">
                                    <span class="new-price">{{modalProduct[0].price}} EGP</span>
                                    <!--                                        <span class="old-price">$95.72</span>-->
                                </div>
                                <div class="pro-details-color-wrap">
                                    <span>Color:</span>
                                    <div class="pro-details-color-content">
                                        <ul>
                                            <li v-for="color in modalProduct[0].color" :key="color.color"><a  v-bind:style="{ backgroundColor: color.color }" class="dolly" href="#">dolly</a></li>

                                        </ul>
                                    </div>
                                </div>
                                <div class="pro-details-size">
                                    <span>Size:</span>
                                    <div class="pro-details-size-content">
                                        <ul>
                                            <li><a href="#">XS</a></li>
                                            <li><a href="#">S</a></li>
                                            <li><a href="#">M</a></li>
                                            <li><a href="#">L</a></li>
                                            <li><a href="#">XL</a></li>
                                        </ul>
                                    </div>
                                </div>
                                <div class="pro-details-quality">
                                    <span>Quantity:</span>
                                    <div class="cart-plus-minus">
                                        <input class="cart-plus-minus-box" type="text" name="qtybutton" value="1">
                                    </div>
                                </div>
                                <div class="product-details-meta">
                                    <ul>
                                        <li><span>Categories:</span> <a href="#">{{modalProduct[0].categories.name}}</a></li>
                                        <li><span>Tag: </span> <a v-for="tag in modalProduct[0].tags" :key="tag.name" href="#">{{tag.name}},</a> </li>
                                    </ul>
                                </div>
                                <div class="pro-details-action-wrap">
                                    <div class="pro-details-add-to-cart">
                                        <a title="Add to Cart" href="#">Add To Cart </a>
                                    </div>
                                    <div class="pro-details-action">
                                        <a title="Add to Wishlist" href="#"><i class="icon-heart"></i></a>
                                        <a title="Add to Compare" href="#"><i class="icon-refresh"></i></a>
                                        <a class="social" title="Social" href="#"><i class="icon-share"></i></a>
                                        <div class="product-dec-social">
                                            <a class="facebook" title="Facebook" href="#"><i class="icon-social-facebook"></i></a>
                                            <a class="twitter" title="Twitter" href="#"><i class="icon-social-twitter"></i></a>
                                            <a class="instagram" title="Instagram" href="#"><i class="icon-social-instagram"></i></a>
                                            <a class="pinterest" title="Pinterest" href="#"><i class="icon-social-pinterest"></i></a>
                                        </div>
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
        name: "ModalTest",
        data: function () {
            return {
                photoSelect:""
            }
        },
        computed: {
            modalProduct: function () {
                // `this` points to the vm instance
                return this.$store.state.modalProduct;
            },
            photo: {
                get: function() {
                    if(this.photoSelect=="")
                        return this.$store.state.modalProduct[0].firstImg;

                    return this.photoSelect
                },
                set: function (newValue) {
                    this.photoSelect =  newValue
                }


            }
        },


    }
</script>

<style scoped>

</style>