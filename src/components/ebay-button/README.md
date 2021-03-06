# ebay-button

## ebay-button Usage

```marko
<ebay-button>text</ebay-button>
```

## ebay-button Attributes

Name | Type | Stateful | Required | Description
--- | --- | --- | --- | ---
`priority` | String | No | No | "primary" / "secondary" (default) / "delete" / "none"
`size` | String | No | No | "large" (default: "none")
`no-text` | Boolean | No | No | used to adjust padding for "expand" variant without text
`href` | String | No | No | for link that looks like a button
`fluid` | Boolean | No | No |
`disabled` | Boolean | Yes | No |
`partially-disabled` | Boolean | No | No |
`transparent` | Boolean | Yes | No | optional, to add Skin classes "transparent"
`variant` | String | No | No | optional, to alter Skin classes: "expand" / "fake-link" / "delete"
`fixed-height` | Boolean | No | No | fixes the height based on `size`
`truncate` | Boolean | No | No | will truncate the text of the button onto a single line, and adds an ellipsis, when the button's text overflows
`badge-number` | Number | No | No | used as the number to be placed in the badge
`badge-aria-label` | String | No | Yes (only if badge number is provided) | passed as the `aria-label` directly to the badge

## ebay-button Events

Event | Data | Description
--- | --- | ---
`button-click` | `{ originalEvent }` | click or action key pressed (space and enter)
`button-escape` | `{ originalEvent }` | escape key pressed
