# AnimeGANv2    

## Requirements  
- python 3.6  
- tensorflow-gpu 1.15.0
- opencv  
- tqdm  
- numpy  
- glob  
- argparse  
- onnxruntime (If onnx file needs to be run.)  
  
## Usage  
### 1. Inference  
  > `python test.py  --checkpoint_dir  checkpoint/generator_Hayao_weight  --test_dir dataset/test/HR_photo --save_dir Hayao/HR_photo`  
    
    
### 2. Train 

#### 1. Download vgg19      

#### 2. Create Train/Val Photo dataset  

#### 3. Do edge_smooth  
  > `python edge_smooth.py --dataset Hayao --img_size 256`  

#### 4. Train  
  >  `python train.py --dataset Hayao --epoch 101 --init_epoch 10`  
  
#### 5. Extract the weights of the generator  
  >  `python get_generator_ckpt.py --checkpoint_dir  ../checkpoint/LightAnimeGAN_Shinkai --style_name Shinkai`  
  
