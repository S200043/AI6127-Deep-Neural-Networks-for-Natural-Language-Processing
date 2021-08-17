'AI6127-A3-G2002341D.ipynb' contains the code used for Q1a.  

Source code in 'word_language_model' folder used for Q1e.  

These are the command lines used for training the models:  
python main.py --cuda --model Transformer --epochs 10 --emsize 512 --nhid 1024 --nlayers 6 --nhead 8 --save model_1.pt  
python main.py --cuda --model Transformer --epochs 10 --emsize 512 --nhid 1024 --nlayers 3 --nhead 8 --save model_2.pt  
python main.py --cuda --model Transformer --epochs 10 --emsize 256 --nhid 1024 --nlayers 6 --nhead 8 --save model_3.pt  
python main.py --cuda --model Transformer --epochs 10 --emsize 512 --nhid 1024 --nlayers 6 --nhead 4 --save model_4.pt  
python main.py --cuda --model Transformer --epochs 10 --emsize 512 --nhid 512 --nlayers 6 --nhead 4 --save model_5.pt  
python main.py --cuda --model Transformer --epochs 10 --emsize 512 --nhid 1024 --nlayers 6 --nhead 8 --label-smoothing 0.1 --save model_6.pt  
python main.py --cuda --model Transformer --epochs 10 --emsize 512 --nhid 1024 --nlayers 6 --nhead 8 --no-attention-scaling --save model_7.pt  
python main.py --cuda --model Transformer --epochs 10 --emsize 512 --nhid 1024 --nlayers 6 --nhead 8  --lr 2.0 --save model_8.pt  

This is the command line used for training a baseline model using the original 'word_language_model' code:  
python main.py --cuda --model Transformer --epochs 10 --emsize 512 --nhid 1024 --nlayers 6 --nhead 8 --save model_default.pt  

The original 'word_language_model' code is available here:  
https://github.com/pytorch/examples/tree/master/word_language_model  

Model training logs are saved in the 'word_language_model' folder and their specific command line saved as the first line.
