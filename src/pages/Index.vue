<template>
    <section class="page-section">
        <!-- header -->
        <Header />

        <!-- form content -->
        <MainSection />

        <!-- about section-->
        <About />

        <!-- Presenting ICICI -->
        <PresentationVedio />
        <!--  -->

        <!-- Scheme Features -->
        <SchemeFeatures />

        <!-- Scheme Performance -->
        <!-- pending scroll view -->
        <SchemePerformance />
        <!--  -->

        <!-- Fund Manager -->
        <FundManager />

        <!-- Footer -->
        <Footer />
    </section>
</template>

<script>
import Header from '~/components/Header';
import MainSection from '~/components/MainSection';
import About from '~/components/About';
import SchemeFeatures from '~/components/SchemeFeatures';
import SchemePerformance from '~/components/SchemePerformance';
import PresentationVedio from '~/components/PresentationVedio';
import FundManager from '~/components/FundManager';
import Footer from '~/components/Footer';
export default {
    components: {
        Header,
        MainSection,
        About,
        SchemeFeatures,
        SchemePerformance,
        PresentationVedio,
        FundManager,
        Footer
    }
};
</script>

<style>
.page-section{
    overflow-x: hidden;
}

.default-section{
    margin: 3rem 0px;
    width: 100%;
}

.w-147 {
    max-width: 147px;
}
.w-570 {
    width: 570px;
}
.w-476 {
    max-width: 476px;
}
.h-516 {
    min-height: 516px;
}
.h-337 {
    height: 337px;
}
.h-445 {
    min-height: 485px;
}
.fs-12 {
    font-size: 0.75rem;
}
.fs-16 {
    font-size: 1rem;
}
.fs-18 {
    font-size: 1.125rem;
}
.fs-20 {
    font-size: 1.25rem;
}
.fs-24 {
    font-size: 1.5rem;
}
.fs-26 {
    font-size: 1.625rem;
}

.fs-42 {
    font-size: 2.625rem;
}
.fs-46 {
    font-size: 2.875rem;
}
.h-746 {
    max-height: 46.625rem;
}
.fw-600 {
    font-weight: 600;
}
.fw-700 {
    font-weight: 700;
}
.fw-800 {
    font-weight: 800;
}
.fw-500 {
    font-weight: 500;
}
.bg-orange {
    background-color: #fb8423;
}
.text-orange {
    color: #fb8423;
}
.text-light-blue {
    color: #174082;
}
.bg-dark-blue {
    background-color: #174082;
}
</style>
