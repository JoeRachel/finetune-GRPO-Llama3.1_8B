# finetune-GRPO-Llama3.1_8B
PPO

![image.png](attachment:2c70a031-bf5d-4d3a-aab8-cd4d80a7e1d3:image.png)

At is the advantage based on the on the rewards {𝑟≥𝑡} and a learned value function 𝑉

---

GRPO

GRPO相比较于PPO，GRPO舍弃了value model 和用GAE计算A（advantage）的方式

GRPO将KL作为**正则**了加入到了Loss中，应该是防止训练模型和参考模型的概率偏差太大，作为一个惩罚项

![image.png](attachment:5bc3a0d5-3954-41c5-9682-d0ad37dc92f0:image.png)

![image.png](attachment:96d4385a-988e-4a9e-8443-8795c3c7a2aa:image.png)

![image.png](attachment:987739aa-f448-4317-9492-377790223c0c:image.png)

减去了一个保证为正数（positive）的惩罚项
