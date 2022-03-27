## Firefox Styling

### Tree Style Tab:

```css
/* Show close button on hover */
#tabbar tab-item:not(:hover) tab-closebox {display: none}

/* Hide tree child count */
#tabbar tab-counter {display: none}

#tabbar tab-item {
  --tab-size: 30px !important;
  height: var(--tab-size);
}

#tabbar tab-item tab-favicon {
  margin-right: 5px
}

.new-tab-popup {
  border: none
}
```

### chrome/userChrome.css:

```css
@namespace url(http://www.mozilla.org/keymaster/gatekeeper/there.is.only.xul);

/* Hide horizontal tab toolbar */
#TabsToolbar {visibility: collapse !important}

/* Hide "Tree Style Tabs" sidebar header */
#sidebar-box[sidebarcommand="treestyletab_piro_sakura_ne_jp-sidebar-action"] #sidebar-header {display: none}

/* Hide tab tooltip */
#remoteBrowserTooltip {display: none}
```

### chrome/userContent.css:

```css
/* Hide scrollbars */
:root{scrollbar-width: none}
```
