# Annotation Guidelines

## Classes
| Class ID | Name | Definition |
|----------|------|------------|
| 0 | pod_healthy | No visible lesions, mold, or water-soaked areas |
| 1 | pod_diseased | Brown water-soaked patches >2cm, white/pink mold, or dark sunken spots |

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
| Small black specks only (<5mm) | healthy | Likely insect damage, not fungal |
| Yellow pod with brown streaks | diseased | Water-soaked tissue = Phytophthora entry |
| Shriveled, fully dried brown pod | diseased | End-stage rot; still counts for burden estimate |
| White lime wash on bark near pod | do not label | Not a pod |
