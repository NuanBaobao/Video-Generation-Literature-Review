# 目录

## 2605
- [PV- VAE：Video Generation with Predictive Latents](https://arxiv.org/abs/2605.02134)
- [LongLive-2.0: An NVFP4 Parallel Infrastructure for Long Video Generation](https://arxiv.org/abs/2605.18739)

## 2601
- [StableWorld: Towards Stable and Consistent Long Interactive Video Generation](https://arxiv.org/abs/2601.15281)

## 2512
- [Reward Forcing: Efficient Streaming Video Generation with Rewarded Distribution Matching Distillation](https://arxiv.org/abs/2512.04678)
- [Pretraining Frame Preservation in Autoregressive Video Memory Compression](https://arxiv.org/abs/2512.23851)
- [SSVAE：Delving into Latent Spectral Biasing of Video VAEs for Superior Diffusability](https://www.arxiv.org/abs/2512.05394)
- [Resampling Forcing:End-to-End Training for Autoregressive Video Diffusion via Self-Resampling](https://arxiv.org/abs/2512.15702)

## 2511
- [StreamDiffusionV2: A Streaming System for Dynamic and Interactive Video Generation](https://arxiv.org/abs/2511.07399)
- [InfinityStar: Unified Spacetime AutoRegressive Modeling for Visual Generation (NeurIPS 25 Oral)](https://arxiv.org/abs/2511.04675)

## 2510
- [Self-Forcing++: Towards Minute-Scale High-Quality Video Generation](https://arxiv.org/abs/2510.02283)

## 2509
- [LongLive: Real-time Interactive Long Video Generation](https://arxiv.org/abs/2509.22622)
- [DC-VideoGen: Efficient Video Generation with Deep Compression Video Autoencoder](https://arxiv.org/abs/2509.25182)
- [Rolling Forcing: Autoregressive Long Video Diffusion in Real Time](https://arxiv.org/abs/2509.25161)
- [SANA-Video: Efficient Video Generation with Block Linear Diffusion Transformer (ICLR 2026 Oral)](https://arxiv.org/abs/2509.24695)

## 2507
- [Geometry Forcing: Marrying Video Diffusion and 3D Representation for Consistent World Modeling](https://arxiv.org/abs/2507.07982)

## 2506
- [Sparse-vDiT: Unleashing the Power of Sparse Attention to Accelerate Video Diffusion Transformers](https://arxiv.org/abs/2506.03065)
- [Self Forcing: Bridging the Train-Test Gap in Autoregressive Video Diffusion](https://arxiv.org/abs/2506.08009v1)
- [Context as Memory: Scene-Consistent Interactive Long Video Generation with Memory Retrieval(SIGGRAPH Asia 25)](https://arxiv.org/abs/2506.03141)
- [Autoregressive Adversarial Post-Training for Real-Time Interactive Video Generation(NeurIPS 25)](https://arxiv.org/abs/2506.09350)

## 2501
- [VideoReward:Improving Video Generation with Human Feedback](https://arxiv.org/abs/2501.13918)
- [Cosmos World Foundation Model Platform for Physical AI](https://arxiv.org/abs/2501.03575)

## 2412
- [CausVid: From Slow Bidirectional to Fast Autoregressive Video Diffusion Models(CVPR 2025)](https://arxiv.org/abs/2412.07772)
- [NOVA：Autoregressive Video Generation without Vector Quantization (ICLR 25)](https://arxiv.org/abs/2412.14169)

## 2410
- [Progressive Autoregressive Video Diffusion Models (CVPRW 2025)](https://arxiv.org/abs/2410.08151)

## 2408
- [GameNGen: Diffusion Models Are Real-Time Game Engines (ICLR 2025)](https://arxiv.org/abs/2408.14837)

## 2407
- [SEED-Story: Multimodal Long Story Generation with Large Language Model](https://arxiv.org/abs/2407.08683)
- [Diffusion Forcing: Next-token Prediction Meets Full-Sequence Diffusion (NeurIPS 2024)](http://arxiv.org/abs/2407.01392)
- [Live2Diff: Live Stream Translation via Uni-directional Attention in Video Diffusion Models](https://arxiv.org/abs/2407.08701)

## 2406
- [ViD-GPT: Introducing GPT-style Autoregressive Generation in Video Diffusion Models](https://arxiv.org/abs/2406.10981)

## 2405
- [FIFO-Diffusion: Generating Infinite Videos from Text without Training (NeurIPS 2024)](https://arxiv.org/abs/2405.11473)
- [Looking Backward: Streaming Video-to-Video Translation with Feature Banks (ICLR 2025)](https://arxiv.org/abs/2405.15757)

## 2403
- [StreamingT2V: Consistent, Dynamic, and Extendable Long Video Generation from Text (CVPR 2025)](https://arxiv.org/abs/2403.14773)

## 2402
- [Rolling Diffusion Models](https://arxiv.org/abs/2402.09470)

## 2312
- [StreamDiffusion: A Pipeline-level Solution for Real-time Interactive Generation](https://arxiv.org/abs/2312.12491)

## 2311
- [ART⋅V: Auto-Regressive Text-to-Video Generation with Diffusion Models](https://arxiv.org/abs/2311.18834)

---
# 2605
## PV- VAE：Video Generation with Predictive Latents
[https://arxiv.org/abs/2605.02134](https://arxiv.org/abs/2605.02134)


<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2026/png/26304400/1778210872322-291dfcf4-2bb8-468b-a497-e1ccd39984c8.png" width="50%">
</p>

**训练 Video VAE 时随机丢弃后半部分 future frames，只把前面的 observed frames 输入 encoder；然后用 padding latents 补齐 latent 序列长度，交给 decoder 同时重建已观察帧和预测被丢弃的未来帧；另外加入一个 temporal-difference / motion-aware loss，避免模型只优化静态像素拷贝。**

****

## LongLive-2.0: An NVFP4 Parallel Infrastructure for Long Video Generation
[**https://arxiv.org/abs/2605.18739**](https://arxiv.org/abs/2605.18739)

****

# 2601
## StableWorld: Towards Stable and Consistent Long Interactive Video Generation
[https://arxiv.org/abs/2601.15281](https://arxiv.org/abs/2601.15281)

指出长时交互式视频生成中的“场景坍塌”主要源于同一场景内逐帧漂移的累积，并提出一种与模型无关的动态帧淘汰机制，通过 ORB 几何一致性保留早期干净帧、丢弃退化帧，从源头抑制误差传播，从而在几乎不增加推理开销的情况下显著提升长期稳定性与一致性。


# 2512
## Reward Forcing: Efficient Streaming Video Generation with Rewarded Distribution Matching Distillation
[https://arxiv.org/abs/2512.04678](https://arxiv.org/abs/2512.04678)


## Pretraining Frame Preservation in Autoregressive Video Memory Compression
[https://arxiv.org/abs/2512.23851](https://arxiv.org/abs/2512.23851)

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2026/png/26304400/1767603405208-14540ae1-8884-4ac7-bedc-9b1b2f568e5e.png" width="50%">
</p>


视频生成需要参考历史信息，长度和质量是个trade off，它相当于是将历史帧信息作了压缩，不一样的地方在于 如果一个视频压缩模型能在“极短上下文”中，仍然高质量地重建任意历史帧，那么它就是一个好的 AR memory。  于是问题定义为 视频上下文压缩 ≈ 任意时间点帧的高保真检索（frame retrieval）问题  。

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2026/png/26304400/1767603634059-3bdfd35c-5760-4465-82cd-d2956810e66a.png" width="50%">
</p>

如何去做这个事情？随机选择一些帧作为Diffusion目标，然后压缩的历史帧作为条件做训练，可以做到通过短上下文来得到任意帧的高保真图像；

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2026/png/26304400/1767603874456-71ce5059-a75f-4151-83c7-fab0408732d4.png" width="50%">
</p>

如果去做生成，就将历史帧换为压缩后的作为条件

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2026/png/26304400/1767706299020-a46e98d2-ec28-43db-809c-a37c18b635ea.png" width="50%">
</p>

## SSVAE：Delving into Latent Spectral Biasing of Video VAEs for Superior Diffusability
[https://www.arxiv.org/abs/2512.05394](https://www.arxiv.org/abs/2512.05394)


## Resampling Forcing:End-to-End Training for Autoregressive Video Diffusion via Self-Resampling
<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1766556118911-e2892cbe-a411-403b-b3a6-a4fbb4de7f9c.png" width="50%">
</p>

[https://arxiv.org/abs/2512.15702](https://arxiv.org/abs/2512.15702)

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1766556143661-2251a1d7-ef78-464f-b184-f4bdd8305b16.png" width="50%">
</p>

一是使用模型估计出的干净图作为历史帧信息来减少teacher forcing带来的误差累积，二是为了减少计算，使用top_k的方式来挑选部分帧内容作为上下文；

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1766556375090-098b19be-9b62-4380-b2fa-36bdd8a37362.png" width="50%">
</p>

其伪代码如下

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1766556422459-2ffa17ce-7ad7-4bc0-b305-e36227ed17be.png" width="50%">
</p>

# 2511
## StreamDiffusionV2: A Streaming System for Dynamic and Interactive Video Generation
[https://arxiv.org/abs/2511.07399](https://arxiv.org/abs/2511.07399)

## InfinityStar: Unified Spacetime AutoRegressive Modeling for Visual Generation (NeurIPS 25 Oral)
[https://arxiv.org/abs/2511.04675](https://arxiv.org/abs/2511.04675)

### **contribution:**
1. **inherits the architecture and knowledge of a trained continuous video tokenizer**

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1762486294682-7f92abac-2d1f-4b92-8a92-8574e9d0aa93.png" width="50%">
</p>

使用预训练的视频tokenizer作为基础，引入二值量化进行微调

2. **To alleviate the imblanced distribution on different scales, it discared the last scales with a probalility (computional  overhead)**

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1762486778497-c4f48a49-a8a0-406b-b607-797394189a1c.png" width="50%">
</p>

训练tokenizer的时候随机的把后面的大scale进行忽略，是的可以依靠前面的小scale信息就可以重建视频内容

3. **due to early scales determine the semantic of video, it refine every earlier scales multiple rounds **
4. **Spacetime Sparse Attention: for long video generation, it’s necessary to attend history tokens to achieve temporal consistency**

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1762493972937-506cf41a-7f0f-45ef-ac6e-9e5b3d5e8690.png" width="50%">
</p>


### **Method:**
<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1762494131836-46931858-9fb2-4257-89e6-da6245fbb377.png" width="50%">
</p>


<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1762485716600-ac8ebbba-4ce1-4e9e-b2bb-d17bf71bcdb3.png" width="50%">
</p>

# 2510
## Self-Forcing++: Towards Minute-Scale High-Quality Video Generation
[https://arxiv.org/abs/2510.02283](https://arxiv.org/abs/2510.02283)

# 2509
## LongLive: Real-time Interactive Long Video Generation
[https://arxiv.org/abs/2509.22622](https://arxiv.org/abs/2509.22622)

[https://github.com/NVlabs/LongLive](https://github.com/NVlabs/LongLive)

[https://nvlabs.github.io/LongLive/](https://nvlabs.github.io/LongLive/)

## DC-VideoGen: Efficient Video Generation with Deep Compression Video Autoencoder
[https://arxiv.org/abs/2509.25182](https://arxiv.org/abs/2509.25182)

[https://github.com/dc-ai-projects/DC-VideoGen](https://github.com/dc-ai-projects/DC-VideoGen)

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1760259966929-030b8f68-dba3-4bd1-9412-0d9956cd46d3.png" width="50%">
</p>

引入DC-VideoGen，一个后训练加速框架，适用于任何预训练的视频扩散模型，通过深度压缩潜在空间和轻量级微调来提高效率。

+ 使用DC-AE-V（深度压缩视频自动编码器），采用块因果时间设计，实现空间和时间上的压缩，同时保持重建质量。
+ 使用AE-Adapt-V，一种稳健的适应策略，使预训练的扩散模型快速适应新潜在空间。

参考：革新视频生成速度的秘密武器！英伟达最新DC-VideoGen：超高清生成实现近15倍加速 - AI生成未来的文章 - 知乎

[https://zhuanlan.zhihu.com/p/1959530356026906371](https://zhuanlan.zhihu.com/p/1959530356026906371)


## Rolling Forcing: Autoregressive Long Video Diffusion in Real Time
[https://arxiv.org/abs/2509.25161](https://arxiv.org/abs/2509.25161)

[https://kunhao-liu.github.io/Rolling_Forcing_Webpage/](https://kunhao-liu.github.io/Rolling_Forcing_Webpage/)


## SANA-Video: Efficient Video Generation with Block Linear Diffusion Transformer (ICLR 2026 Oral)
[https://arxiv.org/abs/2509.24695](https://arxiv.org/abs/2509.24695)

[https://nvlabs.github.io/Sana/Video/](https://nvlabs.github.io/Sana/Video/)


# 2507
## Geometry Forcing: Marrying Video Diffusion and 3D Representation for Consistent World Modeling
[https://arxiv.org/abs/2507.07982](https://arxiv.org/abs/2507.07982)

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1766987860566-cccedb70-16b7-466b-8048-9e02d1efe3f5.png" width="50%">
</p>

# 2506
## Sparse-vDiT: Unleashing the Power of Sparse Attention to Accelerate Video Diffusion Transformers
[https://arxiv.org/abs/2506.03065](https://arxiv.org/abs/2506.03065)

首先这个可视化attention计算量的图片很有用，可以参考一下用在自己的论文里面

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1749092440956-81a9a235-f212-46ef-865e-96c7ed420677.png" width="50%">
</p>


 旨在加速视频扩散模型 vDiT 的推理过程。作者发现其注意力机制中存在**输入无关的结构性冗余**，如重复的注意力模式。基于这一观察，提出了**离线稀疏搜索与融合策略**，将部分注意力替换为高效的稀疏实现。在多个主流视频生成模型上，Sparse-vDiT 实现了**约 2× 的加速，且几乎无质量损失**。  

## Self Forcing: Bridging the Train-Test Gap in Autoregressive Video Diffusion
[https://arxiv.org/abs/2506.08009v1](https://arxiv.org/abs/2506.08009v1)


### **动机：Exposure Bias的本质缺陷**
1. **训练-推理分布失配**
    - **问题根源**：传统自回归视频扩散模型（如Teacher Forcing/Diffusion Forcing）在训练时依赖**真实帧**作上下文（图1a-b），但推理时需基于**自身生成的不完美帧**预测后续帧，导致误差累积（图5对比）。
    - **后果**：时序误差放大（如CausVid模型饱和度漂移），长视频生成质量显著下降（表2：TF/DF模型切换帧级AR时质量骤降）。
2. **实时性瓶颈**
    - 现有双向扩散模型（如Wan2.1）因全局注意力机制无法实现低延迟推理（表1：103秒/视频），而传统自回归模型虽支持流式生成，但缺乏高效KV缓存机制（图3b：滑动窗口需重复计算）。


<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1750140709936-cf4257eb-d58d-4bdf-99ce-1a2d9670c850.png" width="50%">
</p>

### **创新点：自我推演训练范式**
#### **1. 自回归推演与KV缓存训练（图1c）**
+ **核心机制**： 
    - 训练时模拟推理过程：**基于自生成帧**（而非真实帧）预测下一帧，通过**梯度截断+随机步长采样**（Algorithm 1）平衡计算效率。
    - 引入**训练阶段KV缓存**（图2c）：消除传统因果注意力的掩码开销，加速21%（图6左）。
+ **数学形式化**：  
直接优化完整视频分布对齐：`\min_\theta D\left( p_{\text{data}}(x^{1:N}) \| p_\theta(x^{1:N}) \right)`取代传统逐帧分布匹配（3.3节）。

#### **2. 视频级分布匹配损失**
+ **损失设计**： 

| 方法 | 原理 | 优势 |
| --- | --- | --- |
| **DMD** | 反向KL散度最小化 | 稳定收敛（表2） |
| **SiD** | Fisher散度优化 | 避免分数估计偏差 |
| **GAN** | 对抗判别器匹配生成分布 | 提升视觉细节真实性 |


+ **关键改进**：  
对比CausVid的DF+DMD方案（匹配错误分布），Self Forcing确保**训练与推理分布一致**（3.3节分析）。

#### **3. 滚动KV缓存（Rolling KV Cache）**
+ **长视频生成优化**（图3c）： 
    - 动态维护最近L帧的KV嵌入，淘汰旧帧缓存（Algorithm 2）。
    - **复杂度**：从O(TL²) → O(TL)（3.4节），10秒视频生成达16.1 FPS（表1）。
+ **训练适配**：  
限制注意力窗口模拟长视频场景，消除首帧依赖导致的闪烁伪影（图7对比）。


图示关联：

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1750140709928-034a7dc4-0615-45a1-b100-7c17c8805576.png" width="50%">
</p>


## Context as Memory: Scene-Consistent Interactive Long Video Generation with Memory Retrieval(SIGGRAPH Asia 25)
[https://arxiv.org/abs/2506.03141](https://arxiv.org/abs/2506.03141)

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1761878865973-1ab6eeef-1b5c-4c57-b0e9-c51f1d72569f.png" width="50%">
</p>


## Autoregressive Adversarial Post-Training for Real-Time Interactive Video Generation(NeurIPS 25)
[https://arxiv.org/abs/2506.09350](https://arxiv.org/abs/2506.09350)

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1761879240736-3f579bb0-dab2-4495-be98-16875aedcf9c.png" width="50%">
</p>


# 2501
## VideoReward:Improving Video Generation with Human Feedback
[https://arxiv.org/abs/2501.13918](https://arxiv.org/abs/2501.13918)

## Cosmos World Foundation Model Platform for Physical AI
[https://arxiv.org/abs/2501.03575](https://arxiv.org/abs/2501.03575)


# 2412
## CausVid: From Slow Bidirectional to Fast Autoregressive Video Diffusion Models(CVPR 2025)
[https://arxiv.org/abs/2412.07772](https://arxiv.org/abs/2412.07772)

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1766991563794-c9d8bfdb-984e-42d0-9db6-b2e5e4534253.png" width="50%">
</p>


## NOVA：Autoregressive Video Generation without Vector Quantization (ICLR 25)
[https://arxiv.org/abs/2412.14169](https://arxiv.org/abs/2412.14169)

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1762484733835-c4b7a06a-b118-416e-a1d1-2329e88fa31a.png" width="50%">
</p>


<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1762484759657-1d3a9343-1377-40c8-a62f-081aaa585031.png" width="50%">
</p>


# 2410
## Progressive Autoregressive Video Diffusion Models (CVPRW 2025)
[https://arxiv.org/abs/2410.08151](https://arxiv.org/abs/2410.08151)


# 2409
## PhysGen: Rigid-Body Physics-Grounded Image-to-Video Generation
# 2408
## GameNGen: Diffusion Models Are Real-Time Game Engines (ICLR 2025)
[https://arxiv.org/abs/2408.14837](https://arxiv.org/abs/2408.14837)

# 2407
## SEED-Story: Multimodal Long Story Generation with Large Language Model
[https://arxiv.org/abs/2407.08683](https://arxiv.org/abs/2407.08683)

<p align="center">
<img src="https://cdn.nlark.com/yuque/0/2025/png/26304400/1761878995489-8b9c5a1e-3dda-45f2-be13-2a1523c100f7.png" width="50%">
</p>

## Diffusion Forcing: Next-token Prediction Meets Full-Sequence Diffusion (NeurIPS 2024)
[http://arxiv.org/abs/2407.01392](http://arxiv.org/abs/2407.01392)


## Live2Diff: Live Stream Translation via Uni-directional Attention in Video Diffusion Models
[https://arxiv.org/abs/2407.08701](https://arxiv.org/abs/2407.08701)

[https://live2diff.github.io/](https://live2diff.github.io/)

# 2406
## ViD-GPT: Introducing GPT-style Autoregressive Generation in Video Diffusion Models
[https://arxiv.org/abs/2406.10981](https://arxiv.org/abs/2406.10981)

# 2405
## FIFO-Diffusion: Generating Infinite Videos from Text without Training (NeurIPS 2024)
[https://arxiv.org/abs/2405.11473](https://arxiv.org/abs/2405.11473)


## Looking Backward: Streaming Video-to-Video Translation with Feature Banks (ICLR 2025)
[https://arxiv.org/abs/2405.15757](https://arxiv.org/abs/2405.15757)


# 2403
## StreamingT2V: Consistent, Dynamic, and Extendable Long Video Generation from Text (CVPR 2025)
[https://arxiv.org/abs/2403.14773](https://arxiv.org/abs/2403.14773)

# 2402
## Rolling Diffusion Models
[https://arxiv.org/abs/2402.09470](https://arxiv.org/abs/2402.09470)


# 2312
## StreamDiffusion: A Pipeline-level Solution for Real-time Interactive Generation
[https://arxiv.org/abs/2312.12491](https://arxiv.org/abs/2312.12491)


# 2311
## ART**⋅**V: Auto-Regressive Text-to-Video Generation with Diffusion Models
[https://arxiv.org/abs/2311.18834](https://arxiv.org/abs/2311.18834)
