# Prepare datasets

If you have a dataset directory, you could use os environment variable named `FARN_DATADIR`. Under this directory, FARN will look for datasets in the structure described below, if needed.
```
$FARN_DATADIR/
  COCO/
```
You can set the location for builtin datasets by
```shell
export FARN_DATADIR=/path/to/your/datasets
```
If `FARN_DATADIR` is not set, the default value of dataset directory is `./datasets` relative to your current working directory.

## Expected dataset structure for COCO style:

```
FARN/
  annotations/
    instances_{train,val}2017.json
  {train,val}2017/
    # image files that are mentioned in the corresponding json
```

You can use the 2014 version of the dataset as well.
