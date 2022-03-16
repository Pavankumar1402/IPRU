<template>
    <section class="about-section" >
        <div class="container ">
            <div class="row g-4 align-items-lg-center">
                <div class="col-sm-12 col-md-10 col-xl-6 order-1 order-xl-2 px-lg-5">
                    <h3 class="fs-20">{{ aboutData[0].name }}</h3>
                    <h1 class="lh-base text-light-blue fs-46 fw-600 pe-lg-5">
                        {{ aboutData[0].title }}
                    </h1>
                    <p class="lh-lg fs-16 text-justify pe-lg-5">
                        {{ aboutData[0].description }}
                    </p>
                </div>
                <div
                    class="col-sm-12 col-md-10 col-xl-6 order-2 order-xl-1"
                >
                    <img
                        src="../assets/Images/banner-02.png"
                        alt="BlueChip-Fund-image"
                        class="shadow"
                        width="100%"
                    />
                </div>
            </div>

            <!-- about section 2-->
            <div class="row g-4 mt-2">
                <div
                    class="col-sm-12 col-md-10 col-xl-6"
                    v-for="(data, i) in boxAboutData"
                    :key="i"
                >
                    <div
                        class="card shadow"
                        :class="[data.bgColor, data.textColor]"
                    >
                        <div class="card-body px-lg-5">
                            <img
                                :src="data.src"
                                alt="BlueChip-Fund-image"
                                class="mt-4"
                            />
                            <h3 class="fs-26 lh-lg">
                                {{ data.title }}
                            </h3>
                            <p class="fs-16 lh-lg">
                                {{ data.description }}
                            </p>
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
            aboutData: [
                {
                    name: 'ABOUT',
                    title: 'ICICI Prudential ब्लूचिप फ़ंड',
                    description:
                        '23 मई, 2008 को लॉन्च किया गया ICICI Prudential ब्लूचिप फ़ंड एक ओपन-एंडेड इक्विटी स्कीम है, जो मुख्य रूप से लार्ज कैप स्टॉक में निवेश करती है। ये लार्ज कैप कंपनियाँ दरअसल जाने-माने ब्रांड हैं, जिनका अब तक का ट्रैक रिकॉर्ड और क्वॉलिटी मैनेजमेंट कमाल का रहा है और ये भारत के व्यावसायिक दिग्गजों में शामिल हैं। इस स्कीम का मकसद निवेशकों के पोर्टफ़ोलियो को विकास के साथ-साथ स्थिरता प्रदान करना है और अशांत आर्थिक परिस्थितियों में यह निवेश का एक अच्छा विकल्प साबित हो सकता है।'
                }
            ],
            boxAboutData: [
                {
                    src: require('../assets/Images/scheme.png'),
                    title: 'स्कीम की मुख्य विशेषताएँ',
                    description:
                        'यह स्कीम विभिन्न क्षेत्रों में लार्ज कैप स्टॉक में निवेश करती है और “खरीदने और रोककर रखने” का तरीका अपनाती है। स्टॉक का चुनाव बॉटम-अप (नीचे से ऊपर की ओर) तरीका अपनाते हुए किया जाता है, ताकि पक्का हो सके कि चुने हुए स्टॉप लंबे समय तक बढ़त की उचित संभावना दर्शाते हैं। बेंचमार्क से जुड़े रहने का तरीका अपनाकर यह पक्का किया जा सकता है कि पोर्टफ़ोलियो विभिन्न क्षेत्रों में विविधतापूर्वक फैला हुआ है',
                    textColor: 'text-white',
                    bgColor: 'bg-dark-blue'
                },
                {
                    src: require('../assets/Images/investment.png'),
                    title: ' निवेश क्यों करना चाहिए?',
                    description:
                        ' यह स्कीम ऐसे निवेशकों के लिए सही है, जो ब्लूचिप (कंप्यूटर उद्योग) स्टॉक में निवेश करना चाहते हैं, जो अपने-अपने उद्योग बाज़ार की अग्रणी कंपनियाँ हैं। यह स्कीम अलग-अलग क्षेत्रों और थीमों में विविध तरीकों से निवेश करने की सहूलियत भी देती है। लंबी दौड़ में धनार्जन करने के इरादे से निवेश करने वाले निवेशक इस स्कीम में निवेश करने का विकल्प चुन सकते हैं।',
                    textColor: '',
                    bgColor: ''
                }
            ]
        };
    }
};
</script>

<style>
.about-section{
    margin: 3rem 0px;
    width: 100%;
    float: left;
}
</style>
