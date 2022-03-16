<template>
    <section class="default-section">
        <div class="container">
            <div class="row my-5">
                <div class="col-sm-12 col-md-10 col-xl-6">
                    <h1 class="text-light-blue">Fund Manager</h1>
                </div>
            </div>
            <div class="row my-5">
                <div class="col-md-4" v-for="(data, i) in FundManager" :key="i">
                    <div class="card shadow mb-3">
                        <div class="card-body text-center">
                            <div>
                                <img
                                    :src="data.src"
                                    :alt="data.UserName"
                                    class="my-3"
                                />
                                <h3 class="mb-4 mt-3 text-light-blue">
                                    {{ data.UserName }}
                                </h3>
                            </div>
                            <div class="row">
                                <div class="col border-end px-4">
                                    <h3 class="text-light-blue fw-700">
                                        {{ data.years }}
                                    </h3>
                                    <p class="fs-12">
                                        {{ data.yearDescription }}
                                    </p>
                                </div>
                                <div class="col px-4">
                                    <h3 class="text-light-blue fw-700">
                                        {{ data.funds }}
                                    </h3>
                                    <p class="fs-12">
                                        {{ data.fundDescription }}
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row g-4 my-5">
                <div class="col-md-4">
                    <div class="card text-white bg-dark-blue p-5 pe-4">
                        <div class="row">
                            <div class="col">
                                <p class="fs-26 fw-500">
                                    This product is suitable for Investors who
                                    are seeking*:
                                </p>
                            </div>
                            <div class="row">
                                <ul class="fs-16 pt-2 ps-5 pe-0">
                                    <li class="pb-4">
                                        Long term wealth creation
                                    </li>
                                    <li>
                                        An open ended equity scheme
                                        predominantly investing in large cap
                                        stocks.
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 ">
                    <div class="card border-0">
                        <div class="">
                            <img
                                src="../assets/Images/Meter.png"
                                alt="user-image"
                                class="my-3 ps-2"
                            />
                        </div>
                        <div class="">
                            <p class="fs-26 text-light-blue fw-700 ps-2 pe-3">
                                Investors understand that their principal will
                                be at high
                            </p>
                        </div>
                        <div class="">
                            <p class="fs-16 ps-2 pe-5">
                                *Investors should consult their financial
                                distributors if in doubt about whether the
                                product is suitable for them.
                            </p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="">
                        <span class="fs-26 text-light-blue fw-700"
                            >Download</span
                        >
                    </div>
                    <div class="row border-bottom">
                        <div class="col-2">
                            <img
                                src="../assets/Images/pdf.png"
                                alt="user-image"
                                class="my-3"
                            />
                        </div>
                        <div class="col-8">
                            <p class="fs-16 text-start pt-4">
                                Fund Factsheet
                            </p>
                        </div>
                        <div class="col-2 ">
                            <img
                                src="../assets/Images/down-arrow.png"
                                alt="user-image"
                                class="my-3"
                            />
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-2">
                            <img
                                src="../assets/Images/pdf.png"
                                alt="user-image"
                                class="my-3"
                            />
                        </div>
                        <div class="col-8">
                            <p class="fs-16 text-start pt-4">
                                Fund Factsheet
                            </p>
                        </div>
                        <div class="col-2">
                            <img
                                src="../assets/Images/down-arrow.png"
                                alt="user-image"
                                class="my-3"
                            />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            FundManager: [
                {
                    src: require('../assets/Images/user-logo.png'),
                    UserName: 'Vaibhav Dusad',
                    years: '11',
                    yearDescription: 'Years of Experience',
                    funds: '03',
                    fundDescription: 'Funds managed in total'
                },
                {
                    src: require('../assets/Images/user-logo.png'),
                    UserName: 'Rajat Chandak',
                    years: '11',
                    yearDescription: 'Years of Experience',
                    funds: '06',
                    fundDescription: 'Funds managed in total'
                },
                {
                    src: require('../assets/Images/user-logo.png'),
                    UserName: 'Anish Tawakley',
                    years: '24',
                    yearDescription: 'Years of Experience',
                    funds: '05',
                    fundDescription: 'Funds managed in total'
                }
            ]
        };
    }
};
</script>

<style></style>
