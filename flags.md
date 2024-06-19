# Vivaldi Flags
In order to modify flags, you must access `vivaldi://flags` via the address bar.

## Privacy and Security

### Enabled
* #block-insecure-private-network-requests
* #disable-process-reuse
	* When enabled, out-of-process iframes will not try to reuse compatible processes from unrelated tabs, which might decrease performance. 
* #disallow-doc-written-script-loads
	* Enabling it breaks `--blink-settings="preferredColorScheme=1"`
* #enable-isolated-sandboxed-iframes
* #enable-web-bluetooth-new-permissions-backend
	* Go to `vivaldi://settings/all/` and disable the permission for "Bluetooth devices"
	* On Android, Go to Settings → Site Settings → Bluetooth → disable the permission
* #enable-webrtc-hide-local-ips-with-mdns
* #strict-origin-isolation
* #third-party-storage-partitioning

### Disabled
* #clipboard-unsanitized-content
* #enable-fenced-frames
* #enable-generic-sensor-extra-classes
* #enable-webusb-device-detection
* #enable-winrt-geolocation-implementation
	* You might need to enable it for Maps
* #media-router-cast-allow-all-ips
* #system-keyboard-lock
* #web-share

---

## Usability
### Enabled
* #enable-force-dark
	* Personal preference
* #enable-tab-audio-muting
* #extensions-menu-access-control
* #sharing-desktop-screenshots

### Disabled
* #in-product-help-demo-mode-choice
* #smooth-scrolling
* #username-first-flow-store-several-values
* #username-first-flow-with-intermediate-values
* #username-first-flow-with-intermediate-values-predictions
* #username-first-flow-with-intermediate-values-voting

---

## Performance
### Enabled
* #back-forward-cache - **Enabled force caching all pages (experimntal)**
* #calculate-native-win-occlusion
* #enable-drdc
* #enable-parallel-downloading
* #enable-quic
* #enable-vulkan - Disabled, due to causing completely black web pages and making browsers laggy
	* This flag is enabled by default on some/most devices
	* If you don't experience the same problem, keep this flag default
* #enable-webassembly-lazy-compilation
	* This flag is placebo when JITLess mode and/or Strict Security mode in MS Edge are activated
* #overlay-strategies - **Occluded and unoccluded buffers (single-fullscreen,single-on-top,underlay)**
	* Use this flag for Skylake or newer

**These flags are not intented for every device, but worth testing.**

Forcing them might be a bad idea. Therefore, before using them, please check out the Problems section by typing `vivaldi://gpu` into the address bar (ignore WebGL errors)

* #enable-gpu-rasterization
* #enable-waitable-swap-chain 
	* **Enabled Max 1 Frame** has the **lowest delay** but is most likely to **drop frames**, while **3** has the **highest delay** but is least likely to drop frames.
* #enable-zero-copy
* #ignore-gpu-blocklist
* #use-angle
	* According to the flag's description, using the OpenGL driver as the graphics backend may result in higher performance
	* D3D11 is used by default; D3D12 may improve performance if you are using Windows 10 1709 or newer.


---

## Android
**Note:** These are "special flags" for the Android version of Vivaldi.

### Enabled
* #enable-instant-start - **Enabled**
* #enable-site-isolation-for-password-sites - **Enabled**
* #enable-site-per-process - **Enabled**
* #omnibox-most-visited-tiles - **Enabled**

### Disabled
* #contextual-search-longpress-resolve - **Disabled**
* #related-searches - **Disabled**

### Special flags for other Vivaldi/Chromium forks

#### Brave Browser

These flags are from Nightly builds, some of them might not be available in other builds.

* #brave-adblock-cname-uncloaking - **Enabled**
	* If you notice DNS leak, disable it
* #brave-adblock-cosmetic-filtering - **Enabled**
* #brave-adblock-cosmetic-filtering-child-frames - **Enabled**
* #brave-adblock-csp-rules - **Enabled**
* #brave-adblock-default-1p-blocking - **Enabled**
* #brave-block-screen-fingerprinting - **Enabled**
* #brave-dark-mode-block - **Enabled**
* #brave-de-amp - **Enabled**
* #brave-debounce - **Enabled**
* #brave-domain-block - **Enabled**
* #brave-domain-block-1pes - **Enabled**
* #brave-ephemeral-storage - **Enabled**
* #brave-ephemeral-storage-keep-alive - **Enabled**
* #brave-extension-network-blocking - **Enabled**
* #brave-federated - **Disabled**
* #brave-first-party-ephemeral-storage - **Enabled**
* #brave-reduce-language - **Enabled**
* #brave-speedreader - **Enabled**
* #brave-vertical-tabs - **Enabled**
	* Personal preference; Useful when working with huge amount of tabs
* #restrict-websockets-pool - **Enabled**

Disable these flags incase you don't use them:

* #brave-ipfs - **Disabled**
* #brave-news - **Disabled**
* #native-brave-wallet - **Disabled**
* #skus-sdk - **Disabled**
	* Brave VPN

####  >Ungoogled Chromium
* #extension-mime-request-handling - **Always prompt for install**
* #fingerprinting-canvas-image-data-noise - **Enabled**
* #fingerprinting-canvas-measuretext-noise - **Enabled**
* #fingerprinting-client-rects-noise - **Enabled**

#### Bromite
* #cleartext-permitted - Disabled
	* Disables accessing `http` websites
* #dns-request-partitioning - Enabled
* #num-raster-threads - 4

####Edge Chromium
* #edge-automatic-https - **Enabled**
	* Go to `edge://settings/privacy`, enable `Automatically switch to more secure connections with Automatic HTTPS` and choose `Always switch from HTTP to HTTPS (connection errors might occur more often)`
* #edge-autoplay-user-setting-block-option - **Enabled**
	* Go to `edge://settings/content/mediaAutoplay` and set `Control if audio and video play automatically on sites` to `Block` 
* #edge-enable-bfcache-features - **Enabled**
* #edge-global-media-controls - **Enabled**
* #edge-haptics-api - **Disabled**
* #edge-launch-timings - **Disabled**
* #edge-log-textfield-lag - **Disabled**
* #edge-msb-all-dse - **Disabled**
* #edge-msb-keyword-mode - **Disabled**
* #edge-playready-drm-win10 - **Disabled**
	* Needed for Netflix, Spotify, etc.
* #edge-reduce-user-agent-minor-version - **Enabled**
* #edge-robin - **Enabled**
* #edge-sdsm-emulate-acg - **Enabled**
* #edge-show-feature-recommendations - **Disabled**
* #edge-toast-winrt - **Disabled**
* #edge-widevine-drm - **Disabled**
	* Needed for Netflix, Spotify, etc.
