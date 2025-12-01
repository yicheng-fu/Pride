### Online Query-based Data Pricing with Time-discounting Valuations (ICDE 2024)

##### Repo structure:

    / (root)
      /Ex2_NoisyLinearQuery/      # Experiments on noisy linear query (NLQ) 
          /input                  ## Query features and market value theta
          /Ex2_generator.ipynb    ## Generate different query features and market value theta
          /Ex2_main_exp.ipynb     ## Experiments on exponential time-discounting value
          /Ex2_main_linear.ipynb  ## Experiments on linear time-discounting value  
      /Ex3_Airbnb/                # Experiments on Airbnb dataset
          /input                  ## Query features and market value theta
          /Ex3_generator.ipynb    ## Generate different query features and market value theta
          /Ex3_main_linear.ipynb  ## Experiments on linear time-discounting value
      /Pride_ICDE2024.pdf         # ICDE 2024 Paper PDF
      /README.md                  


##### Take Ex2_main_linear as an example

1. Input:

2. Reader and Time-Discounting Function

3. Main function
- MAB Algorithms (baselines), including
  - Pure: without MAB algorithm for discount factor learning
  - Sliding-window Thompson Sampling (SWTS)
  - Discounted Upper Confidence Bound (DUCB)
  - Biased Upper Confidence Bound (Biased UCB)
  - Biased Thompson Sampling (Biased TS)
- Pricing Process, including
  - Market value feature learning with the Ellipsoid Method
  - Time-discounting trend learning with MAB Algorithms
- Run the process
  - Choose different MAB algorithms for comparison
  - Choose different discount functions for simulation
  - Initialize and record important variables
  - Run the main loop

4. Result
- Visualize results and compare regret ratio


##### If you find this paper somewhat interesting, please cite this :)

    @INPROCEEDINGS{fu2024online,
        author={Fu, Yicheng and Miao, Xiaoye and Peng, Huanhuan and Na, Chongning and Deng, Shuiguang and Yin, Jianwei},
        booktitle={2024 IEEE 40th International Conference on Data Engineering (ICDE)}, 
        title={Online Query-Based Data Pricing with Time-Discounting Valuations}, 
        year={2024},
        volume={},
        number={},
        pages={3449-3461},
        doi={10.1109/ICDE60146.2024.00266}
        }

