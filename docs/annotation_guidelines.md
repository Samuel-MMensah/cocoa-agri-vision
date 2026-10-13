# Annotation Guidelines

## Classes
| Class ID | Name | Definition |
|----------|------|------------|
| 0 | healthy_unripe | Green pods with no major necrotic spots, water-soaked areas, or mold |
| 1 | healthy_ripe | Yellow, orange, or red pods with clean rind — no lesions or rot |
| 2 | diseased_pod | Active disease: black/brown water-soaked patches, white/pink mold, or visible lesions |
| 3 | mummified_pod | Dead, dry, shrunken, blackened pods — no moisture, no mold (fully desiccated) |

## What to Label
- Every pod where >=30% of its surface is visible
- Pods at frame edges if >=50% visible
- Both trunk-grown and branch-grown pods

## What NOT to Label
- Pods hidden behind leaves (>70% occluded)
- Flower buds, cherelles (tiny immature pods <3cm)
- Background objects that are not pods

## Edge Cases
| Scenario | Decision | Reason |
|----------|----------|--------|
| Green pod with small black specks (<5mm) | healthy_unripe | Likely insect damage, not fungal |
| Yellow pod with brown streaks | diseased_pod | Water-soaked tissue = Phytophthora entry |
| Shriveled, fully dried black pod | mummified_pod | End-stage desiccation; no moisture or mold |
| Black pod with white mold growing | diseased_pod | Active infection, not yet fully desiccated |
| White lime wash on bark near pod | do not label | Not a pod |
| Pod with sun-scorch (dry brown patches, no mold) | healthy_ripe | Abiotic damage, not disease |
