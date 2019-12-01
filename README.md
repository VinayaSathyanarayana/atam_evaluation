# Introduction

The Architecture Tradeoff Analysis Method (ATAM) is a method for evaluating software architectures relative to quality attribute goals.
Method evaluations expose architectural risks that potentially inhibit the achievement of an organization’s business goals.

## Usage

1. Use `Architecture_Evaluation_Form_Template_V0.xltm` as a template with Microsoft Office to create new ATAM evaluation work sheet. Tested with MSOffice (c) v16.29.1 for Mac.
2. Use a copy of [Google Sheet](https://drive.google.com/file/d/1csupqoVZB6Gs2Uv4THGreZeTOnarG4KO/view?usp=sharing) to create new ATAM evaluation work sheet.
3. Use `Architecture_Evaluation_Form_Template_V0.ods` Open Office document to create new ATAM evaluation work sheet. Tested with LibreOffice (c) v6.3.3 for Mac. Apache Open Office(c) is not supported.

### Adding New Detail Rows to Quality Attribute Sections

To add an new detail row with Microsoft(c), use the `Duplicate Row` button after opening the document when macros are enabled.

LibreOffice or Google Sheet uses `Named Ranges` to aggregate the *detail points* of each `Quality Attribute`. To avoid the need of extending the `Named Ranges` while adding a detail row use **add new rows before** option. Once new row is added copy the formula for `Qualifier` and `Full Qualifier` from adjacent row manually.

## Process

All of the above options are developed based on [ATAM](https://resources.sei.cmu.edu/library/asset-view.cfm?assetid=513908).

This document can be used within the process defined by ATAM. ATAM process participants can complete this document while completing ATAM process mentioned in [ATAM](https://resources.sei.cmu.edu/library/asset-view.cfm?assetid=513908).

_Step 5. Generate quality attribute utility tree._ The work sheet has the most quality attributes that are commonly found in modern software applications. These can be found under `User Perspective` and `Developer Perspective`sheets. ATAM participants should update not applicable `Quality Attributes` for architecture in `User Perspective` and `Developer Perspective` sheets under `Priority` column to `NA` and `Evaluation` column to `Non-Risk`.

_Step 6. Analyze architectural approaches._ During this step, `Non-Risks`, `Risks`, `Sensitivity`, and `Tradeoff` *detail points* are identified and updated under the `Evaluation` (column). The work sheet provides some samples of possible areas to evaluate under each quality attribute.

_Step 7. Brainstorm and prioritise scenarios._ During this step, a priority is assigned to each **detail point**. Use column `Priority` and select a value between `HIGH` to `LOW`.

_Step 8. Analyze architectural approaches._ This step reiterates the activities of Step 6. The participants should modify the sheets accordingly. See more details on [ATAM](https://resources.sei.cmu.edu/library/asset-view.cfm?assetid=513908).

_Step 9. Present results._ The final product architecture qualifier will be presented on `Summary` sheet. This is calculated based on `Risks`, `Sensitivity Points`, and `Tradeoffs` to be fixed.

See `Lists` sheet for descriptions and rank values for summary calculations.

## TODO

A possible improvement is to introduce a weight on `Quality Attributes` importance.
