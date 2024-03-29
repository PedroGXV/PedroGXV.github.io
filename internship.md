---
layout: default
title: "👨‍💻 Pedro"
---

<div class="flex flex-col my-6">

    <div class="flex justify-evenly w-full">
        <div>
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
