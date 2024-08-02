holy shit i understand this now

## Properties

| Prop Name | Type | Description |
| --------------------- | ------ | ------------------- |
| version | number | usually 1 |
| id | string | ID of asset |
| guid | string | GUID of .meta file |
| export | boolean | Whether or not it can be exported(?) |
| tags | string[] | Asset tags, if any |
| plugins | string[] | Manifest.JSON `id`s of plugins affecting the asset. |
| pluginMetadata | {[pluginKey:string]: any} | Plugin metadata affecting the asset |

