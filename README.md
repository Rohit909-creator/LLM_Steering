# LLM_Steering
A trial on the late LLM Steering on Llama 3.1 3B,



Here is the sample output without any steering:
```
Here are some popular and unique places to visit around the world:

**Beach Destinations:**

1. **Bora Bora, French Polynesia**: Overwater bungalows and stunning turquoise lagoon.
2. **The Maldives**: White sandy beaches and crystal-clear waters.

```

Here is the sample output with steering to include only unique places:
```
STEERED GENERATION (Coefficient: 1.0)
============================================================
All steering hooks removed
Steering applied with coefficient: 1.0
Setting `pad_token_id` to `eos_token_id`:128001 for open-end generation.
Here are some popular and interesting places to visit around the world:

**Nature Wonders**

1. Grand Canyon (USA) - One of the most iconic natural wonders in the United States.
2. Great Barrier Reef (Australia) - The world's

============================================================
STEERED GENERATION (Coefficient: 2.0)
============================================================
All steering hooks removed
Steering applied with coefficient: 2.0
Setting `pad_token_id` to `eos_token_id`:128001 for open-end generation.
Here are some popular and breathtaking destinations around the world:

**Nature Wonders:**

1. **Ha Long Bay, Vietnam**: A stunning collection of limestone islands and emerald waters.
2. **Grand Canyon, USA**: One of the most iconic

============================================================
STEERED GENERATION (Coefficient: 4.0)
============================================================
All steering hooks removed
Steering applied with coefficient: 4.0
 Paris, France: Known for its stunning architecture, art museums, and romantic atmosphere.

 Tokyo, Japan: A bustling metropolis with cutting-edge technology, vibrant culture, and delicious food.

 New York City, USA: The city that never sleeps offers iconic

```


So as you can see the steering gets strong with higher coefficients, but the quality of the output also degrades if increased too much.
