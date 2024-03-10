# Items Table
A neatly organized collection of all vanilla items in gm.constants.

---

### Setup and Notes

* Copy the file into your mod folder and require it with `Items = require("./items")`.
* `Items.rarities` is an enum containing `.white`, `.green`, `.red`, `.orange`, `.yellow`, and `.purple`.
* `Items.items` is the main table containing all item data entries.
  * Each item entry is in the format `{name, gm.constant, Item.rarity}`.
  * There are also individual rarity tables (e.g., `Items.white_items`).


### Functions

`Item.get_item_names(rarity)`  
Returns a table containing all item names of a rarity, or all items if none is specified.

`Item.get_item_constants(rarity)`  
Returns a table containing all item gm.constants of a rarity, or all items if none is specified.

`Item.find_item(name_or_const)`  
Returns the table index of the item and its data (two return values), or -1 and nil if the item doesn't exist.
