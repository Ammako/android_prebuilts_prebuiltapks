# Prebuilt APKs

This is a collection of FOSS APKs, coupled with their respective Android.mk for easy integration into the Android build system.

These are the official unmodified prebuilt binaries, signed by their corresponding developers, except for com.google.android.maps; the JAR and the XML have been extracted from the ZIP on the [microG's GitHub release page](https://github.com/microg/android_frameworks_mapsv1/releases).

To include them in your build, just add their name to `CUSTOM_PACKAGES`.

The included APKs are:
 * F-Droid packages (binaries sourced from [here](https://f-droid.org/packages/org.fdroid.fdroid/) and [here](https://f-droid.org/packages/org.fdroid.fdroid.privileged/))
   * F-Droid: a catalogue of FOSS (Free and Open Source Software) applications for the Android platform
   * F-Droid Privileged Extension: a F-Droid extension to ease the installation/removal of apps
 * microG packages (binaries sourced from [here](https://microg.org/download.html) and [here](https://github.com/microg/android_frameworks_mapsv1))
   * GmsCore: the main component of microG, a FOSS reimplementation of the Google Play Services (requires GsfProxy and FakeStore for full functionality)
   * GsfProxy: a GmsCore proxy for legacy GCM compatibility
   * FakeStore: an empty package that mocks the existence of the Google Play Store
   * com.google.android.maps: microG's legacy mapsv1 reimplementation
 * UnifiedNLP backends (binaries sourced from [here](https://f-droid.org/en/packages/org.microg.nlp.backend.ichnaea/) and [here](https://f-droid.org/en/packages/org.microg.nlp.backend.nominatim/))
   * MozillaNlpBackend: Network-based Geolocation module, powered by [Mozilla Location Services](https://location.services.mozilla.com/)
   * NominatimNlpBackend: Address lookup module using MapQuest’s Nominatim service
