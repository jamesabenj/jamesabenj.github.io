---
layout: post
title:      "Using JS to Navigate Radio Button Selections "
date:       2020-08-19 08:41:18 +0000
permalink:  using_js_to_navigate_radio_button_selections
---


For my Javascript portfolio project, I decided to build an interactive quiz, centered around the solar system. Ultimately, the questions took the form of multiple choice radio buttons. 

<iframe src="https://giphy.com/embed/SWzt6FM8BscD484OVk" width="480" height="300" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/SWzt6FM8BscD484OVk">via GIPHY</a></p>

At first, I was a little worried about being able to parse all of the different data points for a user's selected value. There were about 24 questions total, with four options each. I wrestled with organization of 'id' and 'name' attributes that would allow me to select and iterate over a collection in an efficient and 'DRY' way. While I did have to execute this for all 8 planets, the function itself is pretty smooth..
```
function gradeMercury() {
    for(let x = 1; x < 4; x++) {
        let coll = document.querySelectorAll(`input[name="mercury-${x}"]`)
        let selectedValue
        coll.forEach(i => {
            if (i.checked) {
                selectedValue = i.value
            }
        })
        if (selectedValue == coll[4].value) {
            score++ 
        }    
    }
}
```


