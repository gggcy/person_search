Structure-Aware Person Search with Self-Attention and Online Instance Aggregation Matching
## Installation:
1. Clone the person-PyTorch repository

      git clone https://github.com/gggcy/person_search.git
2. Install - if necessary - the required dependencies:

* Python (tested with 3.7 and 3.6)
* PyTorch (conda install pytorch torchvision -c pytorch - tested with PyTorch 0.4, CUDA 9.0 and 9.2)
* Other python dependencies: numpy, scipy, tensorboard etc.
3. Download datasets. *PRW* can be downloaded directly. *CUHK-SYSU* needs to apply to the author's mailbox.
## Training the network 
1. sh `./setup.sh`
2. run `dataset/process_prw.py` & `dataset/process_sysu.py`
3. Download the `VGG/ResNet50` model pretrained on ImageNet
4. run `train.py`. This step takes 20 hours to train *CUHK-SYSU* or 14 hours to train *PRW* (Single 1080ti)
## Testing the network 
* run `test.py`


