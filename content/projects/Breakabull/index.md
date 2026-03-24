---
title: "Breakabull"
summary: "UI and economy focus"
# projects: ["Cooperative", "UI", "Economy", "VR", "Unity"]

showDate : false
showDateUpdated : false
showHeadingAnchors : false
showPagination : false
showReadingTime : false
showTableOfContents : true
showTaxonomies : false 
showWordCount : false
showSummary : true
sharingLinks : false
---
## Summary

Inspired by the phrase "Bull in a China shop" you play as a bull running a tea shop, brewing drinks for adorable animal customers! Running a store on your own comes with a few responsibilities but a bull like you can certainly manage. Easy right? 

I was invited to the team in order to focus on creating and adding the games new economy in alignment with the vision of PO. During this project, I was focused on creating systems such as diagetic computer for buying decorations and ingredients; an economy calculator to more accurately tune game progress to the desired pace; and worked on improving some mesh colliders in the project to allow the player to interact with them more naturally.

**Project Timeline** | January 2026 - May 2026  
**Engine** | Unity  
**Team Size** | 16 Devs

***

## Computer

Since Breakabull had no system to buy ingredients or decorations when I joined the team, I had to create a physical interface to look at and buy items. In order to meet this requirement, I quickly decided that a computer would feel most natural in the setting. Although a variety of control schemes for the computer were explored, a simple arrow key and confirm button layout were selected for their ease of use and familiarity to the user.

![Breakabull](/images/BreakabullComputer.png)

The next focus was the visuals of the store. Due to the fact that there was already a tablet in the game for taking customer orders, I decided to use a similar design style with a sleek and modern appearance.

![Breakabull](/images/StoreWireframe.png)

 The early creation of a wireframe allowed me to quickly create and iterate on how the pages would be handled in engine. Using a three-tiered heirarchy of managers I made an easy-to-use system to quickly add new pages and content within pages. 

![Breakabull](/images/ComputerManager.png) ![Breakabull](/images/PageManager.png) ![Breakabull](/images/InteractableManager.png)

## Economy

When I began to work on the game's economy and progression, I began by speaking to the established members of the team to develop a timeline of when different aspects of the game should be introduced to the player. Using these insights, I began developing a economy calculator which I could use to quickly estimate when items could be bought without needing to test for every tweak. 

![EconCalc](/images/EconCalc.png)

Using a number of variables (customer's appearance probability, order preferences, order prices, etc.), I could calculate the minimum, maximum, and the likely amount of money a player could have at various points in their playthrough. When I changed variables such as ingredient price I would be able to quickly see its affects on player progression and adjust to my liking. 

## Meshes

One of Breakabull's most interesting traits is the inherent clumsiness of not being able to grab objects as you would usually in VR. This introduced a challenge with colliders. To use Unity's physics system a convex mesh is required, however this eliminates the ability to grip an object by its handle. 

![Kettle](/images/origonalmesh.png)

Some plugins were explored to try and replicate a concave collider, but each one tested a noticable impact on performance or collider accuracy.

![Kettle](/images/kettleiteration1.png)
![Kettle](/images/kettleiteration2.png)

After experimenting with optimizing plugins for the game's use case, the kettle and teacup (both small assets), I developed a workflow using Probuilder which allowed for highly accurate colliders without a significant sacrifice in performance quality compared to a single mesh collider.

![Kettle](/images/TeapotHandleFinal.png)
![Teacup](/images/Teacupiteration.png)