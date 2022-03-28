# CMC_final_project
## Step 1: Open the Jingju_Style_Music_generation_with_Feedforward_VAE.ipnb with Colab
## Step 2: Run each block one by one. 
## User-defined parameters: 
Feel free to modify the training parameters：lowest_pitch， n_pitches， expect_len.
If you don't want to train the network, you can skip the training block. Instead, uncomment the lines that can load model in the code block below and then run that code block. 
```
  model = VAE(input_size, h1_dim=h1_dim, h2_dim=h2_dim, h3_dim=h3_dim, z_dim=z_dim).to(device)
  optimizer = torch.optim.Adam(model.parameters(), lr=learning_rate)
  # Uncomment to load previous model
  # checkpoint = torch.torch.load("CMC_final_project/model/best_model_1000epoch_8_beat.pyt",map_location=device)
  # model.load_state_dict(checkpoint['model_state_dict'])
```
## [Demo & Presentation SLides](https://docs.google.com/presentation/d/1cr9diuP46ICYP4gxFeWCh6iDurWOo7xukD--vPwBsYM/edit?usp=sharing)
