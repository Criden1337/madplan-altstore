# madplan-altstore

Public **distribution** repo for the Madplan iOS app. Holds only the compiled `.ipa`
builds (as GitHub Releases) and the AltStore source manifest. The app's **source code is
private** — it lives in the `ios/Madplan/` folder of the `food-planner` repo.

## Add to AltStore / SideStore

Add this source URL in AltStore → **Sources** → **+** :

```
https://raw.githubusercontent.com/Criden1337/madplan-altstore/main/source.json
```

Then install / update **Madplan** from that source. AltStore re-signs the build with your
own Apple ID on install.

Builds are published automatically by the CI workflow in the `food-planner` repo whenever
the `ios/**` files change on `main`.
