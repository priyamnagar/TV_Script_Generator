# TV_Script_Generator
### 
<strong>It generates TV show Sciprt using LSTM neural network with Word2Vec.</strong>

### Dateset
We are using Sienfeld (TV show) Scripts to generate some new ones using LSTM. You can download the dataset from kaggle ( https://www.kaggle.com/thec03u5/seinfeld-chronicles#scripts.csv )

### Model description
Code for the LSTM is provided in the notebook dlnd_tv_script_generation.ipynb. The model is created in the class named RNN.
1. Model Structure
      - It is using Word2Vec Embeddings to create vector representations of words. Embedding dimensions are 200.
      - Hidden layers : 256
      - Number of LSTM layers : 2
      
2. Loss : Cross Entropy Loss

3. Optimizer : Adam optimizer

### Usage
To use the code, execute all the cells in CharRNN.ipynb and send the required arguments in generate function.

      generate(trained_rnn, vocab_to_int[prime_word + ':'], int_to_vocab, token_dict, vocab_to_int[pad_word], gen_length)

      
### How to Contribute
Find any typos? Have another resource you think should be included? Contributions are welcome!

* Fork this repository.

* Clone the repository to your desktop to make changes.

      $ git clone {YOUR_REPOSITORY_CLONE_URL}

* Issue a pull request by clicking on the green pull request icon.

Instead of cloning the repository to your desktop, you can also go to README.md in your fork on GitHub.com, hit the Edit button (the button with the pencil) to edit the file in your browser, then hit the Propose file change button, and finally make a pull request.

### License
This repository has been licensed under Apache 2.0.
