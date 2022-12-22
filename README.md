# Enhancing Melanoma Classifiers with Style Transfer Data Augmentation and Self Supervised Learning

**Ben A. Randoing** \
Stanford University\
bar39@stanford.edu \
sunID: 06270480

**Aastha Jhunjhunwala** \
NVIDIA \
aasthaj@stanford.edu \
sunID: 06733973

**Anirudh Rao** \
Samsung Research America \
anirao26@stanford.edu \
SUID: 06512867 

## Abstract

In the recent past, deep learning methods have gained popularity in classifying melanoma images, however, most of these classifiers are restrained by the use of lighter skin tone images. In this work, the research team explores Neural Style Transfer as a means to generate darker skin tone images to overcome the bias in preexisting datasets, enhance inclusivity and seek performance improvement on diverse skin tone images. Additionally, the use of self-supervised contrastive learning is explored as a pretraining technique to further improve the performance of the learning algorithm. Recall is used as the primary metric to evaluate the model performance. Neural style transfer data augmentation proved effective in improving the baseline recall from 0.623 to 0.787 in melanoma classification on dark-skin tone images using the baseline model. Self-supervised learning in combination with the NST augmentation further improved the recall to 0.813.

## Repository Setup with AWS

1. Start the EC2 Instance
2. Access the instance in a Linux terminal with a command similar to the 
   following which contains a pem to the instance and the Public IPv4 DNS: \
ssh -i ~/.ssh/cs230_aws_keyFinal.pem ubuntu@ec2-34-219-244-118.us-west-2.compute.amazonaws.com
3. Establish a tensorflow environment to ensure the python, CUDA, and cuDNN 
   versions are appropriate for each other. Then activate the environment 
   with conda activate tf.  (https://www.tensorflow.org/install/pip)
4. Check the space on the instance with df -h and potentially add more 
   memory in AWS and reboot before continuing. (https://aws.amazon.com/premiumsupport/knowledge-center/ebs-volume-size-increase/)
5. Follow the instructions in https://www.tensorflow.org/install/pip to 
   ensure the system path is configured.

export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CONDA_PREFIX/lib/

mkdir -p $CONDA_PREFIX/etc/conda/activate.d
echo 'export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CONDA_PREFIX/lib/' > $CONDA_PREFIX/etc/conda/activate.d/env_vars.sh
6. use git clone to clone the repository onto your device. Since the data 
   is absent from this repository, there are two approaches to obtaining 
   data for training the model detiled below. 


## Data Structure in Directory

## 


