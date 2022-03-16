<template>
    <footer class="container-fluid bg-primary">
        <div class="container">
            <div v-if="isSmall" class="bg-primary container py-5">
                <div
                    class="accordion accordion-flush "
                    id="accordionFlushExample"
                >
                    <div class="accordion-item">
                        <h2 class="accordion-header " id="flush-headingOne">
                            <button
                                class="accordion-button text-white bg-primary collapsed"
                                type="button"
                                data-bs-toggle="collapse"
                                data-bs-target="#flush-collapseOne"
                                aria-expanded="false"
                                aria-controls="flush-collapseOne"
                            >
                                <h2 class="fs-16">About Us</h2>
                            </button>
                        </h2>
                        <div
                            id="flush-collapseOne"
                            class="accordion-collapse collapse text-white bg-primary"
                            aria-labelledby="flush-headingOne"
                            data-bs-parent="#accordionFlushExample"
                        >
                            <div class="accordion-body">
                                <ul class="fs-16 list-type-none p-0">
                                    <li class="pt-3">Company Overview</li>
                                    <li class="pt-3">Our Business</li>
                                    <li class="pt-3">Our Leadership</li>
                                    <li class="pt-3">CSR Policy</li>
                                    <li class="pt-3">
                                        Corporate Social Responsibility
                                    </li>
                                    <li class="pt-3">Financials</li>
                                    <li class="pt-3">Media Centre</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="accordion-item">
                        <h2 class="accordion-header" id="flush-headingTwo">
                            <button
                                class="accordion-button collapsed text-white bg-primary"
                                type="button"
                                data-bs-toggle="collapse"
                                data-bs-target="#flush-collapseTwo"
                                aria-expanded="false"
                                aria-controls="flush-collapseTwo"
                            >
                                <h2 class="fs-16">Our Products</h2>
                            </button>
                        </h2>
                        <div
                            id="flush-collapseTwo"
                            class="accordion-collapse collapse text-white bg-primary"
                            aria-labelledby="flush-headingTwo"
                            data-bs-parent="#accordionFlushExample"
                        >
                            <div class="accordion-body">
                                <ul class="fs-16 list-type-none p-0">
                                    <li class="pt-3">Equity Funds</li>
                                    <li class="pt-3">Debt Funds</li>
                                    <li class="pt-3">Hybrid Funds</li>
                                    <li class="pt-3">Others</li>
                                    <li class="pt-3">Solution Oriented</li>
                                    <li class="pt-3">Scheme Comparison</li>
                                    <li class="pt-3">NAV & Dividends</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="accordion-item">
                        <h2 class="accordion-header" id="flush-headingThree">
                            <button
                                class="accordion-button collapsed text-white bg-primary"
                                type="button"
                                data-bs-toggle="collapse"
                                data-bs-target="#flush-collapseThree"
                                aria-expanded="false"
                                aria-controls="flush-collapseThree"
                            >
                                <h2 class="fs-16">Downloads</h2>
                            </button>
                        </h2>
                        <div
                            id="flush-collapseThree"
                            class="accordion-collapse collapse text-white bg-primary"
                            aria-labelledby="flush-headingThree"
                            data-bs-parent="#accordionFlushExample"
                        >
                            <div class="accordion-body">
                                <ul class="fs-16 list-type-none p-0">
                                    <li class="pt-3">Forms</li>
                                    <li class="pt-3">SID KIM SAI</li>
                                    <li class="pt-3">Fund Factsheets</li>
                                    <li class="pt-3">Market Updates</li>
                                    <li class="pt-3">Others</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="accordion-item">
                        <h2 class="accordion-header" id="flush-headingFour">
                            <button
                                class="accordion-button collapsed text-white bg-primary"
                                type="button"
                                data-bs-toggle="collapse"
                                data-bs-target="#flush-collapseFour"
                                aria-expanded="false"
                                aria-controls="flush-collapseFour"
                            >
                                <h2 class="fs-16">Investor Services</h2>
                            </button>
                        </h2>
                        <div
                            id="flush-collapseFour"
                            class="accordion-collapse collapse text-white bg-primary"
                            aria-labelledby="flush-headingFour"
                            data-bs-parent="#accordionFlushExample"
                        >
                            <div class="accordion-body">
                                <ul class="fs-16 list-type-none p-0">
                                    <li class="pt-3">Forms</li>
                                    <li class="pt-3">SID KIM SAI</li>
                                    <li class="pt-3">Fund Factsheets</li>
                                    <li class="pt-3">Market Updates</li>
                                    <li class="pt-3">Others</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="accordion-item">
                        <h2 class="accordion-header" id="flush-headingFive">
                            <button
                                class="accordion-button collapsed text-white bg-primary"
                                type="button"
                                data-bs-toggle="collapse"
                                data-bs-target="#flush-collapseFive"
                                aria-expanded="false"
                                aria-controls="flush-collapseFive"
                            >
                                <h2 class="fs-16">News & Insights</h2>
                            </button>
                        </h2>
                        <div
                            id="flush-collapseFive"
                            class="accordion-collapse collapse text-white bg-primary"
                            aria-labelledby="flush-headingFive"
                            data-bs-parent="#accordionFlushExample"
                        >
                            <div class="accordion-body">
                                <ul class="fs-16 list-type-none p-0">
                                    <li class="pt-3">IPRU Insights</li>
                                    <li class="pt-3">Blogs</li>
                                    <li class="pt-3">Addendums</li>
                                    <li class="pt-3">Press Releases</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                    <div class="accordion-item">
                        <h2 class="accordion-header" id="flush-headingSix">
                            <button
                                class="accordion-button collapsed text-white bg-primary"
                                type="button"
                                data-bs-toggle="collapse"
                                data-bs-target="#flush-collapseSix"
                                aria-expanded="false"
                                aria-controls="flush-collapseSix"
                            >
                                <h2 class="fs-16">App Downloads</h2>
                            </button>
                        </h2>
                        <div
                            id="flush-collapseSix"
                            class="accordion-collapse collapse text-white bg-primary"
                            aria-labelledby="flush-headingSix"
                            data-bs-parent="#accordionFlushExample"
                        >
                            <div class="accordion-body">
                                <ul class="fs-16 list-type-none p-0">
                                    <li class="pt-3 text-orange">IPRUTOUCH</li>
                                    <li class="pt-3 text-orange">
                                        iSave-IPruMF
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div v-else class="bg-primary text-white py-5">
                <div class="row">
                    <div class="col">
                        <h2 class="fs-20 pt-5">About Us</h2>
                        <ul class="fs-16 list-type-none p-0">
                            <li class="pt-3">Company Overview</li>
                            <li class="pt-3">Our Business</li>
                            <li class="pt-3">Our Leadership</li>
                            <li class="pt-3">CSR Policy</li>
                            <li class="pt-3">
                                Corporate Social Responsibility
                            </li>
                            <li class="pt-3">Financials</li>
                            <li class="pt-3">Media Centre</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h2 class="fs-20 pt-5">Our Products</h2>
                        <ul class="fs-16 list-type-none p-0">
                            <li class="pt-3">Equity Funds</li>
                            <li class="pt-3">Debt Funds</li>
                            <li class="pt-3">Hybrid Funds</li>
                            <li class="pt-3">Others</li>
                            <li class="pt-3">Solution Oriented</li>
                            <li class="pt-3">Scheme Comparison</li>
                            <li class="pt-3">NAV & Dividends</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h2 class="fs-20 pt-5">Downloads</h2>
                        <ul class="fs-16 list-type-none p-0">
                            <li class="pt-3">Forms</li>
                            <li class="pt-3">SID KIM SAI</li>
                            <li class="pt-3">Fund Factsheets</li>
                            <li class="pt-3">Market Updates</li>
                            <li class="pt-3">Others</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h2 class="fs-20 pt-5">Investor Services</h2>
                        <ul class="fs-16 list-type-none p-0">
                            <li class="pt-3">Forms</li>
                            <li class="pt-3">SID KIM SAI</li>
                            <li class="pt-3">Fund Factsheets</li>
                            <li class="pt-3">Market Updates</li>
                            <li class="pt-3">Others</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h2 class="fs-20 pt-5">News & Insights</h2>
                        <ul class="fs-16 list-type-none p-0">
                            <li class="pt-3">IPRU Insights</li>
                            <li class="pt-3">Blogs</li>
                            <li class="pt-3">Addendums</li>
                            <li class="pt-3">Press Releases</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h2 class="fs-20 pt-5">App Downloads</h2>
                        <ul class="fs-16 list-type-none p-0">
                            <li class="pt-3 text-orange">IPRUTOUCH</li>
                            <li class="pt-3 text-orange">iSave-IPruMF</li>
                        </ul>
                    </div>
                </div>
            </div>

            <div class="bg-primary text-white border-top py-3">
                <div class="row justify-content-center">
                    <div class="col-xl-8 col-sm-12 order-sm-2 order-2">
                        <div class="d-flex justify-content-evenly">
                            <div>Annual Report.</div>
                            <div>Privacy Policy.</div>
                            <div>Disclaimer.</div>
                            <div>Legal Terms.</div>
                            <div>Tax Reckoner 2020-21</div>
                        </div>
                        <div class="d-flex justify-content-evenly mt-3">
                            <div>Statutory Disclosures.</div>
                            <div>Voting Policy.</div>
                            <div>Sitemap.</div>
                            <div>Terms and Condition.</div>
                            <div>MFConnect</div>
                        </div>
                    </div>
                    <div
                        class="col-xl-4 col-sm-6 text-center order-sm-1 order-1 order-xl-2"
                    >
                        <div class="row">
                            <p class="fs-20">Call us on our Toll Free Number</p>
                            <p class="fs-18">1800-200-6666 / 1800-222-999</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    data() {
        return {
            isSmall: false,
            width: 0
        };
    },
    created() {
        window.addEventListener('resize', this.handleResize);
        this.handleResize();
    },
    methods: {
        handleResize() {
            this.width = window.innerWidth;
            if (this.width <= 768) {
                this.isSmall = true;
            } else {
                this.isSmall = false;
            }
        }
    }
};
</script>

<style>
.list-type-none {
    list-style-type: none;
}
.accordion-button::after {
    background-image: url('../assets/Images/downarrow.png') !important;
    color: aliceblue;
}
</style>
