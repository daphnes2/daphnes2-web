## Exploratory Lab #2: Daphne Stams

*Title*: Explosion of Icelandic Volcano Eldfell on Heimaey Island

*Link to Map*: https://daphnes2.github.io/daphnes2-web/Lab2/lab2volcano.html

![VolcanoMap](https://user-images.githubusercontent.com/97847039/159849938-314c9d76-5680-4296-b8bf-63e2100b5a2d.png)

*Collaborations and reliance on other resources*:

I did a peer map critique with Savi and discussed the following: 

    1) I need to provide more background information about the site. 
    Opening up on a zoomed in island without any information about the space can be disorienting.
    Savi suggested I put hover tags on the town polygon to identify it explicitly as a town. 
    Based on her comments about providing more context, I also decided to make a hover tag for the volcano itself,
    providing more information about the 1973 volcano explosion and the purpose of the map. 
    
    2) Savi also suggested adding a button that would put the user’s input value into the buffer symbol function
    and suggested some ideas on how to do so. After trying this out and having some difficulty I decided to try having
    the input value automatically update the buffer, which is where I also received assistance from professor Bergmann. 

While talking with Savi I was able to give the following suggestion for their map:

    1) They crafted a lovely time slider map about community gardens in vancouver with each year showing a different number
    of community gardens. Although the transition of increasing quantities through the years depicted the upwards trend visually,
    a user would have to stop to count the points to know how many were in each year.
    So I suggested adding a small box that showed the number of community gardens each year. 

To make this map I combined code from previous assignments, experimented with my own code, researched various code examples and guidelines online, and sought assistance from Professor Bergmann regarding the input box and buffer function of my map.

*Reflective Analysis*: 

This map is designed for people interested in the famous eldfell explosion of 1973 that has few extensive measurements made about the extent of the damage. Of the few post-explosion images available, it is evident that large parts of the town were covered in smokey black ash. My map aims to address the lack of information available about the ash coverage of the volcanic explosion by addressing the following questions: 

    1) How can we visualize different extents of ash coverage? 
       What area of town is at risk according to different extents of ash coverage?
    2) Based on ash coverage of the town, what other surrounding areas (island and ocean) would have been impacted? 
    
I think my map is relatively successful in answering both questions. An input box is the main *interface* users could use to manipulate the extent of the ash cover, where the input determines the radius of the ash cover (buffer). If the radi covers part of the town, *feedback* is given by the intersection being highlighted and offering the exact area in both m and km squared when hovered over (area at risk of ash coverage). However, I don’t think my map is fully insightful. It doesn’t provide a grasp on the height of ash coverage and how ash cover would differ on different surfaces, especially in surrounding areas which have different elevations and environments (ex. water bodies). 

To design this map, I used leaflet and turf.js. I first thought about how the map’s *graphic design* and *visual culture* could better facilitate the use of the map’s *user interface design*. To explore the *interface* fully, the user needs to understand the context of the map. About a geographic feature and areas at risk, it is important for the map’s *graphic design* to include a clear base map of the area’s geographic terrain (more specifically ESRI’s World Imagery). The *visual culture* is also intentional, with substantial consideration of color theory when designing the symbols. Red is used to indicate ash cover since red conveys risk, blue to indicate the town as a neutral, contrasting color against red, and purple is used to depict the intersection area at risk, since purple combines both red and blue. Hence the visual cultrue also inplies how the user should understand the map's *feedback*. The map incorporates user *experimentation* by providing users the agency to try out different input levels. Everytime a new input is added, a new ash cover buffer appears and the corresponding town area at risk is provided, listed in area squared. The *affordance* of the map's interactivity is clear because user has instructions and is able to hover over all elements of the map to receive insight, which contextually implies how they should interact with it. The map adds value to current understandings of the 1973 explosion by offering an alternate visualization of the explosion to static visuals shown in limited studies and by allowing users to experiment with possibilities that didn’t exist, such as a volcanic ash coverage that didn’t reach the town or far surpassed the full town.  
This experimentation may reveal various conclusions about the explosions, such as other parts of the island that would've been impacted, which areas would've been possible to conduct evacuation efforts, what denser neighbourhoods suffered more, etc...

There are several ways the map could’ve been improved. After some trial and error, I wasn’t able to get the button working to remove the ash cover buffer after a new input was added. The user has to refresh the page to do so, which limits the *user inferface's* clarity. Additionally, it would’ve been neat to have a toggle option that switches between an overlay of the island in 1973 vs a recent bird’s eye view. It would’ve shown how the town has evolved following the explosion in 1973. I also could have first had the map focus on the whole of Iceland and then zoom onto the island to provide contextual clarity. 

