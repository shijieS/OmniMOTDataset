# Omni-MOT Dataset
> The Omni-MOT  is realistic CARLA based large-scale dataset with over 14M frames for multiple vehicle tracking . The dataset comprises 14M+ frames, 250K tracks, 110 million bounding boxes, three weather conditions, three crowd levels and three camera views in five simulated towns.


## Download

[[baidu]](https://pan.baidu.com/s/1ma0rZIW6vfXeq5tdEk6K2w), [*google drive is not enough*], [*dropbox is also not that enough*]

## Structure

The published dataset comprises five-level structures. At the 1st level, we divide this dataset into the training set and the testing set. At the 2nd level, we employ five towns in the [CARLA Simulator](http://carla.org/). At the 3rd level, we put the camera at different viewpoints containing five difficulty ranks. At the 4th level, we simulate different weathers. At the 5th level, we create a different number of cars.

![](./imgs/DatasetStructure.png)

## Ground Truth

| Index | Name                | Description                                                  |
| ----- | ------------------- | ------------------------------------------------------------ |
| 0     | frame index         | 0\-based frame index                                         |
| 1     | vehicle id          | the unique id of vehicle \(0\-based\)                        |
| 2     | bbox                | represents left, top, right, bottom of the vehicle’s bounding box |
| 6     | 3d bbox             | The 8 points of the vehicle’s 3D bounding boxes in the image coordinate |
| 14    | vehicle position    | the world coordinate of the vehicle’s center in the world coordinate |
| 17    | integrity           | the integrity of the vehicle, value is in \(0, 1\)           |
| 18    | velocity vector     | the velocity vector in the world coordinate\.                |
| 21    | acceleration vector | the acceleration vector in the world coordinate\.            |
| 24    | wheel number        | number of wheels                                             |
| 25    | camera view size    | the width and the height of the camera                       |
| 27    | camera FOV          | the field of view of the camera                              |
| 28    | camera position     | the camera coordinate in the world coordinate                |
| 31    | camera rotation     | the rotation of the camera                                   |
| 34    | weather condition   | the weather condition of current frame\.                     |

## Sample Videos

[![Demo Videos](https://j.gifs.com/mOX0gO.gif)](https://youtu.be/os50DpuM8Ag)

## Cite

```
@inproceedings{ShiJie20,
  author = {Shijie Sun, Naveed Aktar, XiangYu Song, Huansheng Song, Ajmal Mian, Mubarak Shah},
  title = {Simultaneous Detection and Tracking with Motion Modelling for Multiple Object Tracking},
  booktitle = {Proceedings of the European conference on computer vision (ECCV)}},
  year = {2020}

@inproceedings{Dosovitskiy17,
  title = {{CARLA}: {An} Open Urban Driving Simulator},
  author = {Alexey Dosovitskiy and German Ros and Felipe Codevilla and Antonio Lopez and Vladlen Koltun},
  booktitle = {Proceedings of the 1st Annual Conference on Robot Learning},
  pages = {1--16},
  year = {2017}
}
```


## Copyright
- CARLA specific assets are distributed under CC-BY License.
- This dataset is opened and is released under the MIT License. Anyone can extend it. If you your work is based on it, please put the following texts in your description.

- The methods provided on this page are published under the [Creative Commons Attribution-NonCommercial-ShareAlike 3.0 License](http://creativecommons.org/licenses/by-nc-sa/3.0/) . This means that you must attribute the work in the manner specified by the authors, you may not use this work for commercial purposes and if you alter, transform, or build upon this work, you may distribute the resulting work only under the same license. If you are interested in commercial usage you can contact us for further options.


