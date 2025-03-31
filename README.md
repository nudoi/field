# Sample field image

## Copy to local

```
wget -q https://github.com/nudoi/field/raw/refs/heads/main/image/20230925-orthophoto.tif
```

```
wget -q https://github.com/nudoi/field/raw/refs/heads/main/image/20230925-dsm.tif
```

## Loading with Python

```
import pyfieldimager as pfi

orthophoto = '20230925-orthophoto.tif'
dsm        = '20230925-dsm.tif'

fi = pfi.FieldImage(orthophoto=orthophoto, dsm=dsm)
fi.show()
```

<img src="https://github.com/nudoi/field/raw/refs/heads/main/image/readme/20230925-orthophoto.png" width="400">

```
fi.show_dsm()
```

<img src="https://github.com/nudoi/field/raw/refs/heads/main/image/readme/20230925-dsm.png" width="480">
