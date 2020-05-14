# singularity_connectome
singularity container recipe for connectome data analysis. The image has been built and archived in Singularity-hub. Upon further alteration and rebuilding, choose v3 builders as v2 builder will report error if boostrapping from library.

To use prebuilt version, first pull the image by
```
singularity pull [--diable-cache] --name connectome.sif DylanYang7225/singularity_connectome
```
then shell into the image with the local data, output and work directories bind-mounted to the directories /data, /output and /work in the container respectively
```
singularity shell --bind /local_data:/data,/local_output:/output,/local_work:/work connectome.sif
```
