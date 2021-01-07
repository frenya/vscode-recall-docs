---
title: Peeker
icon: fas fa-eye
order: 3
---

This is a nifty little extension I have created to make my life easier when studying a foreign language. 
Peeker is a lightweight tool with a single purpose - quickly lookup currently selected text on a predefined website.

{% gif /assets/img/peeker.gif %}

The demo above uses the Urban Dictionary. For my spanish notes, I use the following config which let's me instantly
look up the definition of any word or phrase in my notes.

```json
{
  "peeker.template": "https://www.spanishdict.com/translate/%s"
}
```

For more information, go ahead and check out the extension [README](https://marketplace.visualstudio.com/items?itemName=frenya.vscode-peeker){:target="_blank"}.
