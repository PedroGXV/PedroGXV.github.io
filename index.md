---
layout: default
title: "👨‍💻 Pedro"
---

<div class="flex flex-col my-6">
    <div class="grid col-6 mb-6">
        {% include components/about-me.html %}
    </div>

    <div class="flex justify-evenly w-full">
        <div>
            <h1 class="topic">
                🧠Knowledge and Experience
                <span class="font-light opacity-60">(resumed)</span>
            </h1>
            
            {% capture web_frameworks %}
                <div class="flex justify-evenly">
                    <img src="/assets/svg/web/laravel.svg" class="h-10 w-12">
                    <img src="/assets/svg/web/rails.svg" class="h-10 w-12">
                    <img src="/assets/svg/web/loco.png" class="h-10 w-10">
                    <img src="/assets/svg/web/nestjs.svg" class="h-10 w-10">
                    <img src="/assets/svg/web/nuxt.svg" class="h-10 w-10">
                </div>
            {% endcapture %}

            {% include components/card.html 
                title="🌐Web Frameworks"
                content=web_frameworks
            %}

            {% capture front %}
                <div class="flex justify-evenly">
                    <img src="/assets/svg/front/react.svg" class="h-10 w-12">
                    <img src="/assets/svg/front/vue.svg" class="h-10 w-12">
                    <img src="/assets/svg/front/tailwind.svg" class="h-10 w-12">
                    <img src="/assets/svg/front/bootstrap.svg" class="h-10 w-12">
                    <img src="/assets/svg/front/vite.svg" class="h-10 w-12">
                </div>
            {% endcapture %}

            {% include components/card.html 
                title="🦄Front End Tools"
                content=front
            %}

            {% capture others %}
                <div class="flex justify-evenly">
                    <img src="/assets/svg/others/docker.svg" class="h-10 w-12">
                    <img src="/assets/svg/others/aws.svg" class="h-10 w-12">
                    <img src="/assets/svg/others/serverless.svg" class="h-10 w-12">
                    <img src="/assets/svg/others/linux.svg" class="h-10 w-12">
                </div>
            {% endcapture %}

            {% include components/card.html 
                title="🛠️Deploy and Other Tools"
                content=others
            %}
        </div>

        <div>
            <h1 class="topic">
                ✍️Blog
            </h1>
            
            {% capture under_construction %}
                <div class="flex justify-center align-center">
                    <span>Under Construction...</span>
                </div>
            {% endcapture %}

            {% include components/card.html 
                title=""
                content=under_construction
            %}
        </div>
    </div>
</div>
