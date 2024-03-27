# FADet
Implementation of 'FADet: A Multi-sensor 3D Object Detection Network based on Local Featured Attention'

![demo](./demo.gif)

## Abstract

## Results

### LiDAR+Cam 3D Object Detection (on nuScenes validation)

### radar+Cam 3D Object Detection (on nuScenes validation)

## Usage

### Prerequisites
Firstly,
```bash
git clone https://github.com/ZionGo6/FADet
```
We recommend to run our FADet in docker container, dockerfile and dependencies are prepared in this repo.
```bash
cd FADet/docker/
```
To build docker image, run:
```bash
./01_build_image.sh
```
Change the parameters inside as you need then run the container:
```bash
./02_run_container.sh
```
In the docker container, run:
```bash
pip install -v -e .
```
## Dataset
We use full nuScenes dataset, please download and process dataset based on [here](https://github.com/open-mmlab/mmdetection3d/blob/master/docs/en/datasets/nuscenes_det.md).
Finally, the data/ should be like this:
```
├── data
│   ├── nuscenes
│   │   ├── maps
│   │   ├── samples
│   │   ├── sweeps
│   │   ├── v1.0-test
|   |   ├── v1.0-trainval
│   │   ├── nuscenes_database
│   │   ├── nuscenes_infos_train.pkl
│   │   ├── nuscenes_infos_val.pkl
│   │   ├── nuscenes_infos_test.pkl
│   │   ├── nuscenes_dbinfos_train.pkl
```
## Train

## Evaluation

## Test
Will release soon
