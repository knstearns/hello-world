---
title: Filters
scope: Global
excerpt: Filters are the quickest way to allow our users to narrow down and find content
contact: Nicki Stearns
private: true
---

<Lead>Effective filters are the quickest way to allow our users to narrow down and find content. Used in many Sprout features, our filters must function consistently for the best user experience.</Lead>

Designing an effective filter experience relies on usage predictability, position consistency and applied filter clarity.

### Be predictable with filter patterns

Filters should be predictable in a way in which our users understand how a filter will function from section to section. In Sprout, filters should be subtractive in functionality.

#### What’s a subtractive filter?

In a subtractive filter model, the users is presented with all results initially, when a filter is applied, the results are narrowed based on the applied filter criteria.

#### Why use this model?

By presenting the users with all results up front, they can more easily narrow their results to the desired outcome.

![Subtractive filter graphic](https://paper-attachments.dropbox.com/s_D42CF92601132384EEB2832119FAACCE5B19BFB62549A77AB33ACD246B1704EA_1554399305870_subtractive.gif)

#### Best practices

- When no filters are applied, all results are displayed
- Results should update dynamically as filters are applied
- Allow users to apply multiple filters at once

### Be consistent with filter position and functionality

Maintaining consistent filter position across Sprout will help our users easily apply filters and find content quickly. When a feature requires filtering, filters should be always be positioned on the same side of the screen and have the ability to be toggled on or off.

![Show/hide filters](https://paper-attachments.dropbox.com/s_D42CF92601132384EEB2832119FAACCE5B19BFB62549A77AB33ACD246B1704EA_1554834546844_hide.gif)

#### Best practices

- Filters should be positioned on the right
    - e.g. a right rail could contain filters or a fly out menu positioned to the right of a title
- Selected filters should always maintain their original position
- Selected and unselected filters should appear within the same list


### Be clear about applied filters

It should be easy for the user to understand how to apply new filters and what filters are currently applied. To ensure users understand what’s applied, we use a combine approach to displaying filter selection.

#### This method is two parts:

1. Showing filters applied in their *original position*, near unapplied filters.
2. Displaying applied filters in a combined *filter token* list at the top of a results stream.

![Applied filter tokens](https://paper-attachments.dropbox.com/s_D42CF92601132384EEB2832119FAACCE5B19BFB62549A77AB33ACD246B1704EA_1554486547872_token.gif)

#### Best practices

- Make sure the user can quickly find currently applied filters
- Make sure the user can easily remove applied filters
- Make sure it’s clear what the current stream of results is being filtered by
- Make tokens persist even when filter panel or menu is hidden

### Behavior

#### Triggering Filters

There are two ways filters could be display in an experience and both will be trigger by a toggle button.

![](https://paper-attachments.dropbox.com/s_D42CF92601132384EEB2832119FAACCE5B19BFB62549A77AB33ACD246B1704EA_1555593139881_right-rail.gif)


Right Rail Filters are contained in a panel that is visible or hidden based on the toggle button state. By clicking the toggle button, the right rail panel will open from right to left and push other page content.


![](https://paper-attachments.dropbox.com/s_D42CF92601132384EEB2832119FAACCE5B19BFB62549A77AB33ACD246B1704EA_1555687143121_hide.gif)


Menu Filters are contained in a menu that is shown or hidden based on the toggle button state. By clicking the toggle button, the menu will open on top of other page content.

#### Applying Filters

To apply filters, the user can select one, several or all filters from a filter list. 

![](https://paper-attachments.dropbox.com/s_D42CF92601132384EEB2832119FAACCE5B19BFB62549A77AB33ACD246B1704EA_1555687152861_applyingfilters.gif)

Clicking a filter will enable the checkbox and display a filter token at the top of the stream of results. Filter tokens should appear in a single line and include a token displayed at the end of the list with a total # count of all filters applied. A max count of filter tokens should be determined for each layout. Filter tokens with long labels should conform to center truncation rules. Filter tokens will persist even when the filter panel or menu is closed.

Clicking an “All…” checkbox will apply all filters from a section. Please see Checkboxes section to learn more about checkbox functionality.

#### Removing Filters

To remove filters, the user can deselect one, several or all filter checkboxes from a filter list, click the “x” icon on a filter token. Or, if applicable, use a “Clear all” to remove all filter tokens applied.

#### “To stick” or “not to stick”

Filters within Sprout should be sticky unless a great user experience need is required. In places, where the user must dedicate time to select their filters, such as Inbox, filters shouldn’t be cleared unless the user initiates it. Use your best judgement to determine when to apply sticky filters in features.

#### Searching Filters

![](https://paper-attachments.dropbox.com/s_D42CF92601132384EEB2832119FAACCE5B19BFB62549A77AB33ACD246B1704EA_1555687165960_search.gif)

When filters hit a maximum of 10, a search bar should appear. The search allows the user to find and quickly apply filters.

#### Grouped Filters

Filters should be grouped into similar categories, *e.g.* by network or type. These grouped filters will be contained in an accordion. The accordion allows the user to expand or collapse relevant filter sets. When a filter set is collapsed the user should see a summary of the selection within.

Example:

![](https://paper-attachments.dropbox.com/s_D42CF92601132384EEB2832119FAACCE5B19BFB62549A77AB33ACD246B1704EA_1555687629100_copy-syntax.png)

- If the user has selected one filter they would see the name of the one item applied
- If the user has selected more than one, they would see “# applied”
- If the user has all or none applied, they would see “All applied”

### Styles & Structure

Appearance of filters should be consistent whether in a right rail panel or menu.

#### Filter Groups

Filter groups should have titles and be contained in accordions.

- Accordion titles should be <Type size='200' />, <Color color='neutral.900' text='Neutral 900' /> and Semibold
- Secondary text should be <Type size='100' />, <Color color='neutral.900' text='Neutral 900' /> and Normal
- Accordion titles may include an icon

Examples:

![](https://paper-attachments.dropbox.com/s_D42CF92601132384EEB2832119FAACCE5B19BFB62549A77AB33ACD246B1704EA_1555689087960_accordion.png)

#### Filter Types

Filters have several configurations depending on app area and content needs.

- “Select All” style filters are text only with <Type size='200' />, <Color color='neutral.900' text='Neutral 900' /> and Semibold text
- “Text” filters are text only with <Type size='200' />, <Color color='neutral.900' text='Neutral 900' /> and Normal
- “Avatar” style filters should include a round avatar sized 24x24 with <Type size='200' />, <Color color='neutral.800' text='Neutral 800' /> and Normal text
- “User” style filters should include user avatars and online/offline status with <Type size='200' />, <Color color='neutral.800' text='Neutral 800' /> and Normal text

Examples:

![](https://paper-attachments.dropbox.com/s_D42CF92601132384EEB2832119FAACCE5B19BFB62549A77AB33ACD246B1704EA_1555689831444_filter-types.png)


#### Filter Button

Filter toggle buttons may include the word “Filter” but will always include the [filter] icon to represent filters.

Examples:

![](https://paper-attachments.dropbox.com/s_D42CF92601132384EEB2832119FAACCE5B19BFB62549A77AB33ACD246B1704EA_1555690168127_filter-buttons.png)



#### Filter Token

Reference [Token](https://sproutsocial.com/seeds/components/token) component page to use.


- Token should have a <Color color='neutral.0' text='Neutral 0' /> fill and <Color color='neutral.800' text='Neutral 800' /> 1px border
- Token on hover should have a <Color color='neutral.100' text='Neutral 100' /> fill and <Color color='neutral.100' text='Neutral 100' /> 1px border
- Text should be <Type size='200' />, <Color color='neutral.800' text='Neutral 800' /> and Normal
- Filter tokens should always include an “x” to remove, except when the token is to show a max count of filters applied
- Token should have a max size of 136px
- Use center truncation rules to accommodate longer text, *e.g.* Group names

Examples:

![](https://paper-attachments.dropbox.com/s_D42CF92601132384EEB2832119FAACCE5B19BFB62549A77AB33ACD246B1704EA_1555692369257_tokens.png)

### Do’s and Don’ts

- **DO:** Use multiple display methods to show applied filters.
- **DO:** Determine a max token count for your feature
- **DO:** Use a single filter type per filter group
- **DO:** Display filters on the right within a feature
- **DON'T:** Display applied filters in a single location.
- **DON'T:** Allow applied tokens to go 2 lines
- **DON'T:** Mix filter types within the same filter group
- **DON'T:** Display filters on the left within a feature

### Related Articles
- [How to Design ‘Applied Filters’ (42% Get It Wrong)](https://baymard.com/blog/how-to-design-applied-filters)
- [How to craft a kickass filtering UX](https://uxdesign.cc/crafting-a-kickass-filtering-ux-beea1798d64b)
- [Defining Helpful Filter Categories and Values for Better UX](https://www.nngroup.com/articles/filter-categories-values/)
- [User Intent Affects Filter Design](https://www.nngroup.com/articles/applying-filters/)
