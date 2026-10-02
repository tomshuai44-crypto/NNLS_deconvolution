# NNLS deconvolution

Fiji / ImageJ plugin for fixed-vector H/DAB color deconvolution using non-negative least squares (NNLS), with optional Gaussian DAB color selection.

- **Version:** 1.1.3 (installation packaging refreshed 2026-10-02; plugin classes unchanged)
- **Contributor:** [tomshuai44-crypto](https://github.com/tomshuai44-crypto)

## Download and install

**Recommended: [Download the installation ZIP](https://github.com/tomshuai44-crypto/NNLS_deconvolution/raw/refs/heads/main/NNLS_Deconvolution_v1.1.3_install.zip).**

1. Extract the ZIP **once**. It contains `NNLS_Deconvolution.jar` and `INSTALL.txt`.
2. Copy the **complete JAR** into your Fiji installation's `plugins` folder. Replace an existing copy.
3. **Do not extract the JAR.** Restart Fiji.
4. Open one RGB brightfield image and select **Plugins → Analyze → NNLS deconvolution**.

Alternatively, [download the JAR directly](https://github.com/tomshuai44-crypto/NNLS_deconvolution/raw/refs/heads/main/NNLS_Deconvolution.jar) and copy it into `plugins` without extracting it.


## Why did I get .class files?

A `.jar` is itself a Java archive. Its normal contents include `.class` files and `plugins.config`. Extracting the JAR shows those internal files; install the intact `.jar` instead. The installation ZIP above wraps the intact JAR so that extracting the ZIP produces the file you need.


Use the download links above. If using GitHub **Code → Download ZIP**, extract that repository ZIP once and locate the intact `NNLS_Deconvolution.jar`; do not extract it again.

The plugin includes its DAB selection module. Python and a network connection are not required to run it. Installation follows [ImageJ's plugin guidance](https://imagej.net/Installing_3rd_party_plugins).

## Verification

Both the JAR and installation ZIP passed archive integrity checks. The JAR includes the plugin entry class, all nested classes, the bundled DAB selector, Fiji menu configuration and a version manifest. Every plugin class is byte-for-byte identical to the previously installed v1.1.3 and targets Java 8. NNLS and integrated DAB selection validation passed using the repackaged JAR, including TIFF save/read checks.

See [SHA256SUMS.txt](SHA256SUMS.txt):

```text
b4142bc3575e8b0f2f2513e43475bd160e92bf4e80b06ae7a466e81cb37ca196  NNLS_Deconvolution.jar
b16b06e042f255ffa498e114dd08dbc4d816055c92d6a4cbed879716ed378097  NNLS_Deconvolution_v1.1.3_install.zip
```
