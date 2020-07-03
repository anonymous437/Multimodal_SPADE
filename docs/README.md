Multimodal SPADE

Requirements:

torch>=1.0.0
torchvision
dominate>=2.3.1
dill
scikit-image

This code also requires the Synchronized-BatchNorm-PyTorch rep.

cd models/networks/
git clone https://github.com/vacancy/Synchronized-BatchNorm-PyTorch
cp -rf Synchronized-BatchNorm-PyTorch/sync_batchnorm .
cd ../../

To train the network

python train.py --name [experiment_name] --dataset_mode custom --label_dir [path_to_labels] -- surface_dir [path_to_surface_images] --color_dir [path_to_rgb_images] --input_dir [path_to_the_network_input] --label_nc [num_labels]
