<template>
    <section class="default-section">
        <div class="container">
            <div class="row">
                <div class="col-sm-12 col-md-10 col-xl-6">
                    <h1 class="text-light-blue fs-46">
                        Presenting ICICI Prudential Bluechip Fund
                    </h1>
                    <p class="fs-16">
                        Watch to learn more about ICICI Prudential Bluechip Fund
                    </p>
                </div>
            </div>
            <div
                v-if="!isSmall"
                class="row rounded-3 flex-nowrap overflow-auto border-bottom pb-5"
            >
                <div class="col-md-4 g-4">
                    <div class="card bg-dark text-white">
                        <img
                            src="../assets/Images/banner-02.png"
                            alt="BlueChip-Fund-image"
                            width="100%"
                            height="331px"
                        />
                        <div class="card-img-overlay">
                            <div class="text-center pt-5 mt-5">
                                <img
                                    src="../assets/Images/Youtube-Icon.png"
                                    alt="BlueChip-Fund-image"
                                    width="82px"
                                    height="60px"
                                />
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 g-4">
                    <div class="card bg-dark text-white">
                        <img
                            src="../assets/Images/banner-02.png"
                            alt="BlueChip-Fund-image"
                            width="100%"
                            height="331px"
                        />
                        <div class="card-img-overlay">
                            <div class="text-center pt-5 mt-5">
                                <img
                                    src="../assets/Images/Youtube-Icon.png"
                                    alt="BlueChip-Fund-image"
                                    width="82px"
                                    height="60px"
                                />
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 g-4">
                    <div class="card bg-dark text-white">
                        <img
                            src="../assets/Images/banner-02.png"
                            alt="BlueChip-Fund-image"
                            width="100%"
                            height="331px"
                        />
                        <div class="card-img-overlay">
                            <div class="text-center pt-5 mt-5">
                                <img
                                    src="../assets/Images/Youtube-Icon.png"
                                    alt="BlueChip-Fund-image"
                                    width="82px"
                                    height="60px"
                                />
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div v-else class="carousel">
                <div class="carousel__item carousel__item--visible">
                    <img
                        src="../assets/Images/banner-02.png"
                        alt="BlueChip-Fund-image"
                        width="100%"
                        height="331px"
                    />
                </div>
                <div class="carousel__item">
                    <img
                        src="../assets/Images/banner-02.png"
                        alt="BlueChip-Fund-image"
                        width="100%"
                        height="331px"
                    />
                </div>
                <div class="carousel__item">
                    <img
                        src="../assets/Images/banner-02.png"
                        alt="BlueChip-Fund-image"
                        width="100%"
                        height="331px"
                    />
                </div>
                <div class="dots">
                    <div class="dot active-dot"></div>
                    <div class="dot"></div>
                    <div class="dot"></div>
                </div>

                <div class="carousel__actions">
                    <button
                        id="carousel__button--prev"
                        aria-label="Previous slide"
                        @click="moveToPrevSlide()"
                    >
                        <
                    </button>
                    <button
                        id="carousel__button--next"
                        aria-label="Next slide"
                        @click="moveToNextSlide()"
                    >
                        >
                    </button>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
const slides = document.getElementsByClassName('carousel__item');
const dots = document.getElementsByClassName('dot');
export default {
    data() {
        return {
            slidePosition: 0,
            totalSlides: 3,
            isSmall: false,
            width: 0
        };
    },
    methods: {
        updateSlidePosition() {
            for (let slide of slides) {
                slide.classList.remove('carousel__item--visible');
                slide.classList.add('carousel__item--hidden');
            }
            for (let dot of dots) {
                dot.classList.remove('active-dot');
            }

            slides[this.slidePosition].classList.add('carousel__item--visible');
            dots[this.slidePosition].classList.add('active-dot');
        },
        moveToNextSlide() {
            if (this.slidePosition === this.totalSlides - 1) {
                this.slidePosition = 0;
            } else {
                this.slidePosition++;
            }

            this.updateSlidePosition();
        },
        moveToPrevSlide() {
            if (this.slidePosition === 0) {
                this.slidePosition = this.totalSlides - 1;
            } else {
                this.slidePosition--;
            }
            this.updateSlidePosition();
        },
        handleResize() {
            this.width = window.innerWidth;
            if (this.width <= 768) {
                this.isSmall = true;
            } else {
                this.isSmall = false;
            }
        }
    },
    created() {
        window.addEventListener('resize', this.handleResize);
        this.handleResize();
    }
};
</script>

<style>
.dots {
    display: flex;
    width: 40px;
    justify-content: space-between;
    align-content: center;
    margin: 0 auto;
}
.dot {
    height: 10px;
    width: 10px;
    border-radius: 50%;
    background: #ccc;
}
.active-dot {
    background: #00f;
}
.not-active-dot {
    background: #ccc;
}
.carousel {
    overflow: hidden;
    max-width: 500px;
    position: relative;
}

.carousel .carousel__item,
.carousel .carousel__item--hidden {
    display: none;
}

.carousel .carousel__item img {
    width: 100%;
    max-width: 500px;
    padding: 30px;
}

.carousel .carousel__item--visible {
    display: block;
    animation: fadeVisibility 0.5s;
}

.carousel .carousel__actions {
    display: flex;
    width: 100%;
    justify-content: space-between;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
}

.carousel .carousel__actions button {
    border-radius: 50px;
    background: none;
    border: 0;
    font-weight: bold;
    cursor: pointer;
    width: 40px;
    height: 40px;
}

.carousel .carousel__actions button#carousel__button--prev {
    margin-left: 0px;
}

.carousel .carousel__actions button#carousel__button--next {
    margin-right: 0px;
}

@keyframes fadeVisibility {
    0% {
        opacity: 0.3;
    }
    100% {
        opacity: 1;
        transform: opacity linear;
    }
}
</style>
