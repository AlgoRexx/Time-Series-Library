## Find out

1. <code>iTransformer</code> : 
- Imagine a standard Transformer as a blender that throws all the ingredients (entire time series sequence) together. 
iTransformer, on the other hand, treats each ingredient (variable) individually, then strategically combines them based on their importance for the final dish (forecast). 
This tailored approach leads to a better understanding of the recipe (time series dynamics) and potentially a more accurate forecast (dish).

- <b>Variable-Length Attention</b>: In contrary attention mechanism in Transformers is typically of fixed-length, meaning it focuses on a limited window around each time step. 
This might not be ideal for capturing long-range dependencies in time series data, which can be crucial for accurate forecasting. 

- [Paper](https://arxiv.org/abs/2310.06625)
- [V 1](https://www.youtube.com/watch?v=4ZuMCam6aj8)
- [V 2](https://www.youtube.com/watch?v=bCz4OMemCcA&t=177s)

2. <code>TimesNet</code> : 
- <b>1D to 2D Transformation</b>: TimesNet transforms one-dimensional (1D) time series data into a two-dimensional (2D) tensor format. 
This allows the model to learn intra-period and inter-period variations simultaneously. 

- <b>Periodicity-specific TimesBlocks</b>: The architecture utilizes custom modules called TimesBlocks. 
Each TimesBlock caters to a specific period in the data, allowing the model to effectively handle patterns unique to different timeframes.
This can be advantageous compared to generic approaches that might miss period-specific trends.

- [Paper](https://openreview.net/pdf?id=ju_Uqw384Oq)
- [V 1](https://www.youtube.com/watch?v=tH3Vig7YYwg&t=110s)
