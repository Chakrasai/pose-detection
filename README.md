# Human Pose Estimation

This repository provides implementation for ***Human Pose Estimation*** that predicts the location of various human keypoints (joints and landmarks) such as elbows, knees, neck, shoulder, hips, chest etc.

## Requirements
- OpenCV
- OpenPose

## Usage
- To download the pretrained models, run `sh get_model.sh` command.
- To run pre-Trained model, trained on ***MPII Human Pose*** dataset, on any image, run the following command:-
`python3 human_pose_estimation.py --input <Image Name> --proto human_pose_proto/mpi/pose_deploy_linevec_faster_4_stages.prototxt --model human_pose_proto/mpi/pose_iter_160000.caffemodel --dataset MPI`.
- To run pre-Trained model, trained on ***COCO*** dataset, on any image, run the following command:-
`python3 human_pose_estimation.py --input <Image Name> --proto human_pose_proto/coco/deploy_coco.prototxt --model human_pose_proto/coco/pose_iter_440000.caffemodel --dataset COCO`.
- To run pre-Trained model, trained on ***Body_25*** dataset, on any image, run the following command:-
`python3 human_pose_estimation.py --input <Image Name> --proto human_pose_proto/body_25/body_25_deploy.prototxt --model human_pose_proto/body_25/pose_iter_584000.caffemodel.

## Results

Following are a few ***human poses*** predicted by the model:-
