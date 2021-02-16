
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Kingston Spotlighting

<!-- badges: start -->
<!-- badges: end -->

This project contains ODK forms and analysis workbooks for Spotlighting
surveys.

## Form development

Forms are located in the folder `inst/extdata/forms`. Forms are built
using ODK Build and post-processed by hand.

-   Open the form files `.odkbuild` from the `inst/extdata/forms` folder
    in [ODK Build](https://build.getodk.org/).
-   Change the form as required.
-   Save the changed form.
-   Export the form to file (`.odkbuild`) and export to XML.
-   Rename the form as found in `inst/extdata/forms` to comply with R
    package requirements.
-   Post process the XML to add form ID / version and start geolocation.
-   Release each new version as draft, send a few submissions, then
    publish the new version.
-   The devices with managed QR codes should automatically load the new
    versions.
-   Communicate any breaking changes to enumerators.
-   Replace the forms in `inst/extdata/forms` with the new versions
    after moving the older versions into dated subfolders (yyyy-mm-dd).

## Data analysis

The vignette “analysis” contains a working example of accessing and
visualising the data. Data is exported by the analysis workbook as CSV
to `inst/extdata/export`.
