# nimes

Pointcloud sample of Nimes Arena

Demo: https://bertt.github.io/nimes/

Blog: https://bertt.wordpress.com/2023/04/14/create-3d-tiles-from-french-lidar-data/

![image](https://user-images.githubusercontent.com/538812/231998312-6e6ea269-d20a-40e8-a2e9-5b8dd0277c3e.png)

Pointcloud source data: https://geoservices.ign.fr/lidarhd#telechargement

Pdal pipeline see [pipeline.json]

![pipeline](https://user-images.githubusercontent.com/538812/231998785-31326390-65be-4b43-88f5-743c6fee4862.png)

Run pipeline using:

```
$ pdal pipeline pipeline.json
```

Create 3DTiles command: 

```
$ gocesiumtiler -srid 2154 -input result.las -output 3dtiles -zoffset 60
```
