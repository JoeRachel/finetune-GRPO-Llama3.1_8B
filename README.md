# finetune-GRPO-Llama3.1_8B

PPO:
At is the advantage based on the on the rewards {𝑟≥𝑡} and a learned value function 𝑉

GRPO:
GRPO相比较于PPO，GRPO舍弃了value model 和用GAE计算A（advantage）的方式

GRPO将KL作为**正则**了加入到了Loss中，应该是防止训练模型和参考模型的概率偏差太大，作为一个惩罚项,减去了一个保证为正数（positive）的惩罚项
