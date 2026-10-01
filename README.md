# LiveSocial Events Page

This repository controls the existing New Menu Events Page in LiveSocialVR.

Each item in `events-page.json` pairs a poster image with the Unity scene that opens when the poster is selected.

```json
{
  "image": "poster-file.jpg",
  "scene": "Exact Unity Scene Name"
}
```

## Updating events

1. Upload the poster image to this repository.
2. Add or update its entry in `events-page.json`.
3. Use the exact scene name already included in the app's Unity Build Settings.
4. Increase `version` whenever an image is replaced without changing its filename.
5. Commit the changes to the `main` branch.

Set `"disabled": true` on an entry to temporarily hide it without deleting it.

GitHub can add, remove, reorder, or redirect posters to scenes already installed in the APK. A completely new Unity scene still requires a new APK build.
