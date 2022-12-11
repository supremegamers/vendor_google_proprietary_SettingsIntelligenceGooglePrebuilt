# Standalone SettingsIntelligenceGooglePrebuilt 

Pulled from : raven-user-12-SP2A.220405.004-8233519-release-keys

Imagine, you usually can make a vanilla build of your favourite custom ROM, but then suddenly the ROM developers decided to merge [pixel-framework](https://github.com/PixelExperience/vendor_pixel-framework) from PixelExperience in. You can still make vanilla build, sure. But then suddenly some part of the Settings like Battery or App Info started to crash. You started to panic and don't know what to do so you just gonna go to the ROM's chat and then saying that the ROM is now Gapps only......

Well no need to panic and being a d***, let this repo help you instead. This repo contains SettingsIntelligenceGooglePrebuilt, some part of [SettingsGoogle](https://github.com/PixelExperience/vendor_pixel-framework/tree/thirteen/SettingsGoogle) require this app including the 2 part that I mentioned above. Just need to clone this repo, follow the instruction and you are good to go. The app doesn't have ABI-specific libraries or require GMS so you don't have to worry to use on vanilla builds.

## Instructions

- Clone this repo, for example I clone to `vendor/google/proprietary/SettingsIntelligenceGooglePrebuilt`

- Add this in your `device.mk`

```
$(call inherit-product-if-exists, vendor/google/proprietary/SettingsIntelligenceGooglePrebuilt/sigp.mk)
```

- Build the ROM and test


### Tested ROM

- BlissOS (or BlissRoms) 15.8.x
