<p align="left" >
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://carbonplan-assets.s3.amazonaws.com/monogram/light-small.png">
  <img alt="CarbonPlan monogram." height="48" src="https://carbonplan-assets.s3.amazonaws.com/monogram/dark-small.png">
</picture>
</p>

# carbonplan / climate risk comparison

## overview

This repository contains code to reproduce a comparison of fire and flood risk scores described in [this](https://carbonplan.org/research/climate-risk-comparison) research article. We recieved the data in response to [a written request](https://github.com/carbonplan/climate-risk-comparison/blob/main/CarbonPlan-Data-Request.pdf) we sent to a set of climate analytics providers.

## data

We received climate risk data from two companies which we make publicly available, with permission, in a public S3 bucket (see below for download links) licensed under [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/).
| Jupiter Intelligence                                                                                                                                                                | XDI                                                                                                                  |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| [Fire risk in California](https://carbonplan-climate-impacts.s3.us-west-2.amazonaws.com/climate-risk-comparison/companies/data/CA-Fire-for-CarbonPlan-Input_CA-Fire-for-CarbonPlan_Enhanced_20240502.csv)     | [Fire risk in California](https://carbonplan-climate-impacts.s3.us-west-2.amazonaws.com/climate-risk-comparison/companies/data/californiainput_merged.xlsx) |
| [Flood risk in New York](https://carbonplan-climate-impacts.s3.us-west-2.amazonaws.com/climate-risk-comparison/companies/data/NY-Flood-for-CarbonPlan-Input_NY-Flood-for-CarbonPlan_Enhanced_20240502.csv) | [Flood risk in New York](https://carbonplan-climate-impacts.s3.us-west-2.amazonaws.com/climate-risk-comparison/companies/data/NYinput_merged.xlsx)       |
|                                                                                                                                                                        |                                                                                                                      |

The companies also shared documentation to support our interpretation of the results: XDI shared a [sample report](https://carbonplan-climate-impacts.s3.us-west-2.amazonaws.com/climate-risk-comparison/companies/methods/X_bank_residential_mortgage_report_XDI.pdf) and Jupiter shared a [technical methodology document](https://carbonplan-climate-impacts.s3.us-west-2.amazonaws.com/climate-risk-comparison/companies/methods/Flood%2BWildfire+Global+Technical+Methodology+Overview+-+v3.1.pdf) and data [schema](https://carbonplan-climate-impacts.s3.us-west-2.amazonaws.com/climate-risk-comparison/companies/methods/Schema+-+ClimateScore+Global+v3.1.xlsx).

## code

The `request_location_selection.ipynb` notebook shows how the locations were selected for the California, New York City, and New York state case studies. The `compare_risk_scores.ipynb` notebook reads in risk data, munges it, writes it out for visualization, and calculates all satistics referenced in the research article.

## about us

CarbonPlan is a non-profit organization that uses data and science for climate action. We aim to improve the transparency and scientific integrity of climate solutions with open data and tools. [Find out more at carbonplan.org](https://carbonplan.org/) or get in touch by [opening an issue](https://github.com/carbonplan/climate-risk-comparison/issues/new) or [sending us an email](mailto:hello@carbonplan.org).
