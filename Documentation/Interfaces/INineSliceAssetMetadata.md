This is an extension of **[ILibraryAssetMetadata.](/Documentation/Interfaces/ILibraryAssetMetadata.md)**

## Properties

| Prop Name | Value | Description |
| --------------------- | ------ | ------------------- |
| imageAsset | string | GUID of nineslice's image. Can also be found under the respective image's META file. |
| borderLeft | number | How offset the nineslice's left border is from the image's left border. <br/> Positive = closer to the center, Negative = further from the center |
| borderTop | number | How offset the nineslice's top border is from the image's top border. <br/> Positive = closer to the center, Negative = further from the center |
| borderRight | number/null | How offset the nineslice's right border is from the image's right border. <br/> Leave blank to have the border be as equidistant from the center as borderLeft.  |
| borderBotton | number/null | How offset the nineslice's bottom border is from the image's bottom border. <br/> Leave blank to have the border be as equidistant from the center as borderTop. |
