# RELLIS-OCC-A-Benchmark-for-Off-Road-Traversability-Aware-Scene-Completion
The data used in this work are derived from the RELLIS-3D dataset. For implementation convenience, we reorganize the data into the following directory structure. Users can download the original image and point cloud data from the RELLIS-3D dataset. Due to the large size of the full dataset, this repository only provides the final label files. The generated labels can be found in `dataset/9_gt_generation_template/preprocess_cost_gt_new/`.

RELLIS-OCC/
├── dataset/
│   ├── 1_os1_cloud_node_kitti_bin/
│   ├── 2_os1_cloud_node_semantickitti_label_id_20210614/
│   ├── 3_vel_cloud_node_kitti_bin/
│   ├── 4_vel_cloud_node_semantickitti_label_id/
│   ├── 5_pylon_camera_node/
│   ├── 6_pylon_camera_node_label_color/
│   ├── 7_pylon_camera_node_label_id/
│   ├── 8_calibration/
│   ├── 9_gt_generation_template/
│   ├── 10_preprocess_output/
│   └── README.md
│
├── data_processing_pipeline/
│   ├── 1_origin_data_preprocess/
│   ├── 2_generate_dense_occupancy/
│   ├── 3_cost_label/
│   └── README.md
│
├── model/
│   ├── monoscene/
│   ├── surroundocc/
│   └── openoccupancy/
│
└── README.md

## Repository Structure

- 'dataset/RELLIS-OCC/': RELLIS-OCC dataset files, calibration data, labels, templates, and preprocessing outputs.
- 'data_processing_pipeline/': Scripts for raw data preprocessing, dense occupancy generation, and cost label generation.
- 'models/': Implementations and adapted code for comparison models, including MonoScene, SurroundOcc, and OpenOccupancy.
