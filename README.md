# UFPR-ALPR Dataset

![Teaser image](./media/samples.png)

This dataset, called UFPR-ALPR dataset, includes 4,500 fully annotated images (over 30,000 LP characters) from 150 vehicles in real-world scenarios where both the vehicle and the camera (inside another vehicle) are moving. It has been introduced in our IJCNN paper [[PDF]](./pdfs/paper.pdf).

The images were acquired with three different cameras and are available in the Portable Network Graphics (PNG) format with a size of 1,920 × 1,080 pixels. The cameras used were: GoPro Hero4 Silver, Huawei P9 Lite, and iPhone 7 Plus.

We collected 1,500 images with each camera, divided as follows:

* 900 of cars with gray LP;
* 300 of cars with red LP;
* 300 of motorcycles with gray LP.

The dataset is split as follows: 40% for training, 40% for testing and 20% for validation. Every image has the following annotations available in a text file: the camera in which the image was taken, the vehicle’s position and information such as type (car or motorcycle), manufacturer, model and year; the identification and position of the LP, as well as the position of its characters. The full details are in our [paper](./pdfs/paper.pdf).

## How to obtain the Dataset

The UFPR-ALPR dataset is released for academic research only and is free to researchers from educational or research institutes for **non-commercial purposes**.

Please click here for more info about obtaining the dataset.

You can now check who is downloading our dataset (see [**here**](https://www.inf.ufpr.br/rblsantos/misc/ufpr-alpr-map/)).

## References

If you use the UFPR-ALPR dataset in your research please cite our paper:

* R. Laroca, E. Severo, L. A. Zanlorensi, L. S. Oliveira, G. R. Gonçalves, W. R. Schwartz, and D. Menotti, “A Robust Real-Time Automatic License Plate Recognition Based on the YOLO Detector” in 2018 International Joint Conference on Neural Networks (IJCNN), July 2018, pp. 1–10.

```
@INPROCEEDINGS{laroca2018robust, 
  author={R. {Laroca} and E. {Severo} and L. A. {Zanlorensi} and L. S. {Oliveira} and G. R. {Gon{\c{c}}alves} and W. R. {Schwartz} and D. {Menotti}}, 
  booktitle={International Joint Conference on Neural Networks (IJCNN)}, 
  title={A Robust Real-Time Automatic License Plate Recognition Based on the {YOLO} Detector}, 
  year={2018}, 
  volume={}, 
  number={}, 
  pages={1-10}, 
  doi={10.1109/IJCNN.2018.8489629}, 
  ISSN={2161-4407}, 
  month={July},
}
```

You may also be interested in our **new research**, where we considerably improved our ALPR system and provided labels for many images from public datasets:

* R. Laroca, L. A. Zanlorensi, G. R. Gonçalves, E. Todt, W. R. Schwartz, D. Menotti, “An Efficient and Layout-Independent Automatic License Plate Recognition System Based on the YOLO Detector,” IET Intelligent Transport Systems, vol. 15, no. 4, pp. 483-503, 2021.

## Additional Results

To enable comparisons with approaches designed specifically for cars (i.e., approaches that do not work for motorcycles), here we separately report the recognition rates obtained on images of cars and motorcycles (see table below). All authors who downloaded the dataset were notified of this update on August 2, 2019.

|        ALPR System       |  Cars | Motorcycles | Cars + Motorcycles |
|:------------------------:|:-----:|:-----------:|--------------------|
|     Sighthound (2018)    | 58.4% |     3.3%    | 47.4%              |
|      OpenALPR (2018)     | 58.0% |    22.8%    | 50.9%              |
|      Proposed (2018)     | 72.2% |    35.6%    | 64.9%              |
| Proposed-Extended (2021) | 95.9% |    66.3%    | 90.0%              |