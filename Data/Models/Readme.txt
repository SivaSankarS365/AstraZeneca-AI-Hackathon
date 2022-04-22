Version 1:
Score : 0.82 
Standard base model from master 
Version 2:
Score : 0.75
Extra convo layer and dense layer
Version 3:
Score: 0.835
Similar to Version-1 but hyper-parameters are optimised
Model Structure:
Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 embedding (Embedding)       (None, 50, 200)           67850200  
                                                                 
 conv1d (Conv1D)             (None, 46, 500)           500500    
                                                                 
 conv1d_1 (Conv1D)           (None, 44, 500)           750500    
                                                                 
 conv1d_2 (Conv1D)           (None, 42, 500)           750500    
                                                                 
 global_max_pooling1d (Globa  (None, 500)              0         
 lMaxPooling1D)                                                  
                                                                 
 flatten (Flatten)           (None, 500)               0         
                                                                 
 dropout (Dropout)           (None, 500)               0         
                                                                 
 dense (Dense)               (None, 256)               128256    
                                                                 
 dropout_1 (Dropout)         (None, 256)               0         
                                                                 
 dense_1 (Dense)             (None, 256)               65792     
                                                                 
 dropout_2 (Dropout)         (None, 256)               0         
                                                                 
 dense_2 (Dense)             (None, 64)                16448     
                                                                 
 dropout_3 (Dropout)         (None, 64)                0         
                                                                 
 dense_3 (Dense)             (None, 64)                4160      
                                                                 
 dropout_4 (Dropout)         (None, 64)                0         
                                                                 
 dense_4 (Dense)             (None, 64)                4160      
                                                                 
 dropout_5 (Dropout)         (None, 64)                0         
                                                                 
 dense_5 (Dense)             (None, 64)                4160      
                                                                 
 dropout_6 (Dropout)         (None, 64)                0         
                                                                 
 dense_6 (Dense)             (None, 32)                2080      
                                                                 
 dense_7 (Dense)             (None, 3)                 99        
                                                                 
=================================================================
Total params: 70,076,855
Trainable params: 70,076,855
Non-trainable params: 0
_________________________________________________________________