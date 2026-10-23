# Astrophotography Journal

A practical notebook for recording DWARF 3 captures, Siril processing decisions, and image comparisons. The goal is to make each result easier to explain and each next session easier to improve.

**Status:** Starter documentation and reusable templates. No image gallery or completed session reports are included in this initial edition. Drafted with AI assistance around my interests in astronomy and careful image processing.

## Working principles

* Preserve the original capture files. Work on copies.
* Record what came from the telescope and what changed during processing.
* Keep conventional image processing separate from intentional artistic styling.
* Inspect a suspected bad exposure before rejecting it, and record the reason.
* Report visible defects and missing information alongside the finished image.

## Suggested project structure

This is a proposed local folder layout, not a list of files already in this repository. Keep large capture files in separate storage and publish only selected, reviewed derivatives.

```text
YYYYMMDD_target/
  originals/
  working/
  exports/
    target_natural_v1.jpg
    target_enhanced_v1.jpg
  capture-log.md
  processing-log.md
  comparison.md
```

Use versioned output names so an improved edit does not erase an earlier result.

## Capture log template

Copy this table for each session. Use "Unknown" when a setting cannot be recovered from the capture record.

| Field | Recorded value |
| --- | --- |
| Session date and time zone | [date and zone] |
| Target and catalog identifier | [target] |
| Telescope | [model] |
| Capture application and version | [version, if known] |
| Filter | [filter or none] |
| Exposure per frame | [seconds] |
| Gain | [value] |
| Frames captured | [count] |
| Frames accepted | [count] |
| Frames rejected and reasons | [count and evidence] |
| Accepted integration time | [minutes] |
| Calibration inputs | [files used, none, or unknown] |
| Source type | [individual exposures or telescope stack] |
| Sky and weather notes | [observations] |
| Source manifest | [file list or reference] |

For equal-length exposures, accepted integration minutes = accepted frame count × seconds per frame ÷ 60. For mixed exposures, sum the accepted exposure durations before dividing by 60.

**Illustrative calculation only:** 80 accepted frames × 15 seconds ÷ 60 = 20 minutes. This is fictional, not a reported capture.

## Processing log template

| Step | Settings or action | Why | Output or observation |
| --- | --- | --- | --- |
| Source inspection | [dimensions, channels, metadata] | Confirm the starting point | [findings] |
| Input preparation | [copies and files selected] | Preserve originals | [working version] |
| Calibration and stacking | [performed, already supplied, or not applicable] | Record provenance | [master reference] |
| Crop | [bounds or none] | [reason] | [dimensions] |
| Background adjustment | [method/settings or none] | [reason] | [observed change] |
| Stretch | [method/settings] | [reason] | [highlight and faint-detail notes] |
| Color adjustment | [method/settings or none] | [reason] | [natural presentation or stylized mapping] |
| Noise and sharpening | [method/settings or none] | [reason] | [detail and artifact notes] |
| Export | [format, dimensions, color profile] | [sharing or further editing] | [output filename] |

Record only the steps actually performed. Do not describe a supplied telescope stack as individually calibrated and restacked unless that work was done. Keep the editable master alongside sharing exports in local storage.

## Comparing two versions

Change one processing choice at a time when possible. Compare the same crop at the same display scale, and record whether the observation is visual or measured.

| Check | Version A | Version B | Evidence and preference |
| --- | --- | --- | --- |
| Bright-region detail | [observation] | [observation] | [crop or measurement] |
| Faint structure | [observation] | [observation] | [same region] |
| Star shape | [observation] | [observation] | [center and corners] |
| Background noise | [observation] | [observation] | [same background region] |
| Color treatment | [description] | [description] | [processing notes] |
| Artifacts | [halos, bands, or none observed] | [findings] | [location] |
| Intended use | [natural presentation or artistic] | [purpose] | [choice and tradeoff] |

A brighter or more saturated edit is not automatically a more detailed one. When using metrics, record the measurement method, image scale, and sampled region so the comparison can be repeated.

## Session summary template

```text
Target:
Session date:
Question explored:
Source files:
Processing version:
What changed:
What improved:
What remains imperfect:
Evidence supporting the comparison:
Next experiment:
```

## Publication checklist

* Verify the image belongs to this session and matches its processing notes.
* Review image and file metadata before sharing.
* Include target, capture settings when known, processing description, and limitations.
* Label artistic color treatments explicitly.
* Keep raw captures and private storage paths outside public notes.

## Next additions

The next useful addition is a documented real session: one selected preview, its verified capture log, and a comparison of two processing versions. This initial repository provides the structure for that work.

[Back to my profile](https://github.com/Marhey)
