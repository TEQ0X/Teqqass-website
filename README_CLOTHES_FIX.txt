CLOTHES UNLOCK FIX
- write_int now keeps 0 and negative IDs (SelectedEquipments -1)
- write_equipment uses presence flag + cleaned int lists
- clothes.json contains male/female wardrobe inventory exported from the designated source account (508 male IDs, 354 female IDs in this export)
- unlock_all_clothes merges those clothes.json inventories into the target account; it fails clearly if the catalog is missing or invalid
- unlock_all_features includes All Clothes

- Dashboard runs wardrobe unlock asynchronously to avoid request timeouts; completion/error is sent to Telegram.
- Existing equipped loadouts are preserved; only inventory slot lists are extended. clothes.json does not contain SelectedEquipments.
