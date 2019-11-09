# Omni-MOT Dataset
> The Omni-MOT  is realistic CARLA based large-scale dataset with over 14M frames for multiple vehicle tracking . The dataset comprises 14M+ frames, 250K tracks, 110 million bounding boxes, three weather conditions, three crowd levels and three camera views in five simulated towns.


## Download

[[baidu]](https://pan.baidu.com/s/1ma0rZIW6vfXeq5tdEk6K2w)

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

<iframe src='//gifs.com/embed/omni-mot-mOX0gO' frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe>


## Cite


## Copyright
- CARLA specific assets are distributed under CC-BY License.
- This dataset is opened and is released under the MIT License. Anyone can extend it. If you your work is based on it, please put the following texts in your description.
```
This dataset is extended from AMOTD. Please cite the following papers:

@inproceedings{Dosovitskiy17,
  title = {{CARLA}: {An} Open Urban Driving Simulator},
  author = {Alexey Dosovitskiy and German Ros and Felipe Codevilla and Antonio Lopez and Vladlen Koltun},
  booktitle = {Proceedings of the 1st Annual Conference on Robot Learning},
  pages = {1--16},
  year = {2017}
}

and 



```

