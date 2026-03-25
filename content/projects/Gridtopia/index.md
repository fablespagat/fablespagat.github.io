---
title: "Gridtopia"
summary: "Unity tool for creating grid based games"
# projects: ["solo", "tool", "Unity"]

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

When I began making my second grid-based game, I decided that I should create a tool to make my process more efficient. Using custom editor programming I began working on Gridtopia, a modular framework for creating/editing tiles, units, levels, and more. As well as streamlining iteration, Gridtopia provides a well-structured architecture for ease of readability and use so tech-debt is minimized and processes can easily be reused between projects.  

**Project Timeline** | December 2025 - Present Day  
**Engine** | Unity  
**Team Size** | Solo dev

***

## Guiding Philosophies
- Modular systems to allow for complete user control
- Reduce required scripting and technical knowledge to a minimum

![Gridtopia overview](/images/Gridtopia1.webp)

## Features
### Implemented
- Automated square and hexagonal grid creation
- Custom window for creating new tile/unit prefabs and scripts
- Composition focused event system for tile/unit behaviours

### In Development
- Tile palette integration for level
- Game phases - turn-based default
- Map generation
- 3D functionality
- AOE designer
- Goldberg Polyhedron

## Example Process
### Grid Creation
{{< carousel images = "GridSetUp/*" interval = "5000" captions = "{Gridtopia2.webp:Add the Gridtopia window, Gridtopia4.webp:Add a grid manager to your scene, Gridtopia5.webp:Select your manager and begin configuring settings}">}}

### Tile/Unit Creation
{{< carousel images = "TileUnitSetUp/*" interval = "5000" captions = "{Gridtopia6.webp:Type in a name to create a copy of a template tile/unit, Gridtopia7.webp:Type in a name to create a script for a new unit behaviour, Gridtopia8.webp:Assign the desired behaviours to the set events}">}}