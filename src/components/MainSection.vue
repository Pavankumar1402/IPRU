<template>
    <section class="main-section">
        
        <div class="container">
            <div
                class="row justify-content-md-center justify-content-sm-center"
            >
                <div
                    class="col-md-6 col-xl-6 col-sm-12 text-left pt-md-5 mt-md-5 px-md-5"
                >
                    <div>
                        <span class="text-white fs-24 fw-700">ICICI Prudential ब्लूचिप फ़ंड</span>
                    </div>
                    <div>
                       <span class="text-white fs-42 fw-800">बड़ी कंपनियों के साथ बढ़ने का मौका</span> 
                    </div>
                    <div>
                    <p class="fs-16 text-white lead">
                        रिलायंस, एचडीएफसी बैंक, इंडस्ट्रीज, मारुति, ब्रिटानिया,
                        सुजुकी, लार्सन एंड टुब्रो, आईटीसी, इंफोसिस
                    </p>
                    </div>
                </div>

                <!-- form -->

                <div class="col-12 col-md-6 pt-2">
                    <div class="card">
                        <div class="card-body m-auto mt-5 px-5">
                            <div class="border-bottom mb-5 pb-3">
                                <p class="fs-20 fw-600">
                                    एक कॉलबैक का अनुरोध करें और हमारे साथ शुरू
                                    करें
                                </p>
                                <div class="d-flex justify-content-between">
                                    <p class="">
                                        क्या आप ICICI Prudential म्युचुअल फ़ंड
                                        के मौजूदा निवेशक हैं?
                                    </p>
                                    <div class="form-check form-switch">
                                        <toggle-checkbox />
                                    </div>
                                </div>
                            </div>
                            <div class="mb-4">
                                <input
                                    type="text"
                                    class="form-control p-2 ps-3 accent-orange"
                                    id="exampleInputEmail1"
                                    aria-describedby="emailHelp"
                                    placeholder="नाम"
                                />
                            </div>
                            <div class="input-group mb-4">
                                <button
                                    class="btn border"
                                    type="button"
                                    data-bs-toggle="dropdown"
                                    aria-expanded="false"
                                >
                                    +91
                                </button>
                                <input
                                    type="text"
                                    class="form-control p-2 ps-3"
                                    aria-label="Text input with dropdown button"
                                    placeholder="मोबाइल"
                                />
                            </div>
                            <div class="mb-4">
                                <input
                                    type="text"
                                    class="form-control p-2 ps-3"
                                    id="phoneNumber"
                                    placeholder="ईमेल"
                                />
                            </div>
                            <div class="mb-4">
                                <input
                                    type="password"
                                    class="form-control p-2 ps-3"
                                    id="InputPassword"
                                    placeholder="शहर"
                                />
                            </div>
                            <div class="mb-5 form-check">
                                <input
                                    type="checkbox"
                                    class="form-check-input"
                                    id="exampleCheck1"
                                />
                                <label
                                    class="form-check-label fs-12"
                                    for="exampleCheck1"
                                >
                                    अपना व्यक्तिगत ब्यौरा डालकर, आप ICICI
                                    Prudential Asset Management Company Ltd
                                    और/या उसके अधिकृत सेवा प्रदाता(ओं) को आपसे
                                    संपर्क करने की इजाज़त देते हैं। यह इजाज़त
                                    देने से NDNC में किए गए आपके रजिस्ट्रेशन के
                                    बावजूद वे आपसे संपर्क कर सकेंगे।
                                </label>
                            </div>
                            <div class="m-auto bg-dark w-147 rounded-pill mb-5">
                                <button
                                    type="submit"
                                    class="btn bg-orange text-white w-100 rounded-pill"
                                >
                                    Submit
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>

import ToggleCheckbox from '~/components/ToggleCheckbox';
export default {
    components: {
       
        ToggleCheckbox
    }
};
</script>

<style>
.main-section{
    background-image: url('../assets/Images/Mask-group.png');
    background-repeat: no-repeat;
    background-size: 100% 92%;
    width: 100%;
    float: left;
    padding-top: 127px;
}

.h-53 {
    height: 3.31rem;
}
</style>
