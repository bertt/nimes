# nimes

Pointcloud sample of Nimes Arena

Pointcloud source data: https://geoservices.ign.fr/lidarhd#telechargement

Pdal pipeline see [pipeline.json]

Run pipeline using:

```
$ pdal pipeline pipeline.json
```

Create 3DTiles command: 

```
$ gocesiumtiler -srid 2154 -input result.las -output 3dtiles -zoffset 60
```