# Train Adapt Optimize
## What is Train Adapt Optimize (TAO) Toolkit?
Train Adapt Optimize (TAO) Toolkit is a python based AI toolkit for taking purpose-built pre-trained AI models and customizing them with your own data. TAO adapts popular network architectures and backbones to your data, allowing you to train, fine tune, prune and export highly optimized and accurate AI models for edge deployment.

The pre-trained models accelerate the AI training process and reduce costs associated with large scale data collection, labeling, and training models from scratch. Transfer learning with pre-trained models can be used for AI applications in smart cities, retail, healthcare, industrial inspection and more.

Build end-to-end services and solutions for transforming pixels and sensor data to actionable insights using TAO, DeepStream SDK and TensorRT. TAO can train models for common vision AI tasks such as object detection, classification, instance segmentation as well as other complex tasks such as pose estimation, facial landmark, gaze estimation, heart rate estimation and others.

## Purpose-built Pre-Trained Models
Purpose-built pre-trained models offer highly accurate AI for a variety of vision AI tasks. Developers, system builders and software partners building intelligent vision AI apps and services, can bring their own custom data and train with and fine-tune pre-trained models instead of going through the hassle of large data collection and training from scratch.

## Running TAO Toolkit
You must provide your credentials and storage information. All other values may be `--set` directly or modified directly in the values.yaml. This will download notebooks, models, and create a jupyter notebook endpoint on a NodePort for user interaction.

```bash 
helm install tao tao \
    --set ngcCredentials.password=<NGC_API_KEY> \
    --set ngcCredentials.email=<NGC_EMAIL> \
    --set modelRepoGenerator.nfs.path=<NFS_PATH> \
    --set modelRepoGenerator.nfs.server=<NFS_DOMAIN_OR_IP>
```