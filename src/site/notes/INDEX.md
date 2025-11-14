---
{"dg-publish":true,"permalink":"/index/","tags":["gardenEntry"]}
---

![compendium.jpg](/img/user/Assets/Images/compendium.jpg)
# Campaign Journal

```search-bar
show recent files
```

----
![[Kesswick#Kesswick\|Kesswick#Kesswick]]
 ___
> [!session|red]-  Sessions<br><span class="sub">*Summaries, Transcripts, & Notes*</span>
> <pre class="dataview dataview-error">Evaluation Error: SyntaxError: Unexpected token '&gt;'
    at DataviewInlineApi.eval (plugin:dataview:19027:21)
    at evalInContext (plugin:dataview:19028:7)
    at asyncEvalInContext (plugin:dataview:19038:32)
    at DataviewJSRenderer.render (plugin:dataview:19064:19)
    at DataviewJSRenderer.onload (plugin:dataview:18606:14)
    at DataviewJSRenderer.load (app://obsidian.md/app.js:1:689336)
    at DataviewApi.executeJs (plugin:dataview:19607:18)
    at DataviewCompiler.eval (plugin:digitalgarden:10763:23)
    at Generator.next (&lt;anonymous&gt;)
    at eval (plugin:digitalgarden:90:61)</pre>

> [!npc|purple]-   NPC's<br><span class="sub">*Non-Player Characters*</span>
> <pre class="dataview dataview-error">Evaluation Error: SyntaxError: Unexpected token '&gt;'
    at DataviewInlineApi.eval (plugin:dataview:19027:21)
    at evalInContext (plugin:dataview:19028:7)
    at asyncEvalInContext (plugin:dataview:19038:32)
    at DataviewJSRenderer.render (plugin:dataview:19064:19)
    at DataviewJSRenderer.onload (plugin:dataview:18606:14)
    at DataviewJSRenderer.load (app://obsidian.md/app.js:1:689336)
    at DataviewApi.executeJs (plugin:dataview:19607:18)
    at DataviewCompiler.eval (plugin:digitalgarden:10763:23)
    at Generator.next (&lt;anonymous&gt;)
    at fulfilled (plugin:digitalgarden:77:24)</pre>

> [!genloc]-  Locations<br><span class="sub">Islands, Settlements, & Places</span>
> <pre class="dataview dataview-error">Evaluation Error: SyntaxError: Unexpected token '&gt;'
    at DataviewInlineApi.eval (plugin:dataview:19027:21)
    at evalInContext (plugin:dataview:19028:7)
    at asyncEvalInContext (plugin:dataview:19038:32)
    at DataviewJSRenderer.render (plugin:dataview:19064:19)
    at DataviewJSRenderer.onload (plugin:dataview:18606:14)
    at DataviewJSRenderer.load (app://obsidian.md/app.js:1:689336)
    at DataviewApi.executeJs (plugin:dataview:19607:18)
    at DataviewCompiler.eval (plugin:digitalgarden:10763:23)
    at Generator.next (&lt;anonymous&gt;)
    at fulfilled (plugin:digitalgarden:77:24)</pre>
>

> [!lore]-  Lore & Mythos<br><span class="sub">Factions, Gods, Relics, & More</span> 
> <pre class="dataview dataview-error">Evaluation Error: SyntaxError: Unexpected token '&gt;'
    at DataviewInlineApi.eval (plugin:dataview:19027:21)
    at evalInContext (plugin:dataview:19028:7)
    at asyncEvalInContext (plugin:dataview:19038:32)
    at DataviewJSRenderer.render (plugin:dataview:19064:19)
    at DataviewJSRenderer.onload (plugin:dataview:18606:14)
    at DataviewJSRenderer.load (app://obsidian.md/app.js:1:689336)
    at DataviewApi.executeJs (plugin:dataview:19607:18)
    at DataviewCompiler.eval (plugin:digitalgarden:10763:23)
    at Generator.next (&lt;anonymous&gt;)
    at fulfilled (plugin:digitalgarden:77:24)</pre>

```base
filters:
  and:
    - file.mtime != null
formulas:
  time_ago: file.mtime.relative()
properties:
  file.name:
    displayName: File
  formula.time_ago:
    displayName: Last Edited
views:
  - type: table
    name: Recently Edited
    filters:
      and:
        - file.ext == "md"
    order:
      - file.name
      - formula.time_ago
    sort:
      - property: formula.time_ago
        direction: DESC
    limit: 5
    columnSize:
      file.name: 375
  - type: cards
    name: View
    cardSize: 130
    imageFit: ""
    imageAspectRatio: 1.2
```

```base
filters:
  and:
    - file.ctime != null
formulas:
  time_ago: file.ctime.relative()
properties:
  file.name:
    displayName: File
  formula.time_ago:
    displayName: Created
views:
  - type: table
    name: Recently Created
    filters:
      and:
        - file.ext == "md"
    order:
      - file.name
      - formula.time_ago
    sort:
      - property: formula.time_ago
        direction: DESC
      - property: file.name
        direction: DESC
    limit: 5
    columnSize:
      file.name: 375
```




 


