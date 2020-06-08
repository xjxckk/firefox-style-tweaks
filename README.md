## Firefox CSS

### Tree Style Tab:

```css
/* Show close on hover */
#tabbar tab-item:not(:hover) tab-closebox {
	display: none;
}

/* Hide tree child count */
#tabbar tab-counter {
	display: none;
}
```

### chrome/userChrome.css:

```css
@namespace url(http://www.mozilla.org/keymaster/gatekeeper/there.is.only.xul);

/* Hide horizontal tab toolbar */
#TabsToolbar {
    visibility:collapse!important;
}

/* Hide "Tree Style Tabs" sidebar header */
#sidebar-box[sidebarcommand="treestyletab_piro_sakura_ne_jp-sidebar-action"] #sidebar-header {
    display:none;
}
```

### chrome/userContent.css:

```css
/* Hide scrollbars */
:root{
  scrollbar-width: none;
}
```
