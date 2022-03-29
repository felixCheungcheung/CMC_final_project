# CMC_final_project: Jingju Style Music generation with Feedforward Variational AutoEncoder
### Technicalities: 
1. Dataset: JingjuMusicScoresCollection-v3
2. Pianoroll representation with limited pitch range
3. Beat as the basic unit of Input: retrieve a fixed length of training samples, hopsize = one beat
4. Three layer of feedforward Variational AutoEncoder was used
5. Output sample visualization and sonification was implemented

### Step 1: Open the Jingju_Style_Music_generation_with_Feedforward_VAE.ipnb with Colab
### Step 2: Run each block one by one. 
### User-defined parameters: 
Feel free to modify the training parameters：lowest_pitch， n_pitches， expect_len.
If you don't want to train the network, you can skip the training block. Instead, uncomment the lines that can load model in the code block below and then run that code block. 
```
  model = VAE(input_size, h1_dim=h1_dim, h2_dim=h2_dim, h3_dim=h3_dim, z_dim=z_dim).to(device)
  optimizer = torch.optim.Adam(model.parameters(), lr=learning_rate)
  # Uncomment to load previous model
  # checkpoint = torch.torch.load("CMC_final_project/model/best_model_1000epoch_8_beat.pyt",map_location=device)
  # model.load_state_dict(checkpoint['model_state_dict'])
```
### Run the code block below extra times to get more result. 
```
# Evaluation
with torch.no_grad():
  wish_len = int(input("Enter the length of music that you want to generate(multiple number of expect_len (4) ):")) 
  generate_len = int(wish_len/ expect_len)
  z = torch.randn(generate_len, z_dim).to(device)
  out = model.decode(z).reshape(z.shape[0],fixed_len,n_pitches)
```

### [Demo & Presentation SLides](https://docs.google.com/presentation/d/1cr9diuP46ICYP4gxFeWCh6iDurWOo7xukD--vPwBsYM/edit?usp=sharing)
### [PresentationVideos](https://drive.google.com/file/d/12ykDJ5q0y-ARi0NoJCNHFz4VEjv2v2UB/view?usp=sharing)
