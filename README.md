# Awesome-Embodied-3D-vision
🎊Welcome to **Awesome-Embodied-3D-Vision**, a comprehensive collection of cutting-edge research papers and resources focused on 3D vision and embodied AI. 

Whether you're a researcher, student, or practitioner, this resource aims to provide a structured gateway to the latest innovations in creating, understanding, and interacting with 3D environments. 

🥺Contributions and suggestions are welcome to keep this collection vibrant and up-to-date!

## Table of Contents
- [Awesome 3D Reconstruction](#awesome-3d-reconstruction)
  - [Neural Radiance Fields](#neural-radiance-fields)
  - [Signed Distance Functions](#signed-distance-functions)
  - [Neural Implicit Surfaces](#neural-implicit-surfaces)
  - [Monocular Geometric Reconstruction](#monocular-geometric-reconstruction)
  - [Visual Geometry Transformers](#visual-geometry-transformers)
  - [Indoor Compositional Reconstruction](#indoor-compositional-reconstruction)
- [Awesome 3D Scene Generation](#awesome-3d-scene-generation)
  - [3D Scene Generation](#3d-scene-generation)
- [Awesome Visual Room Rearrangement](#awesome-visual-room-rearrangement)
  - [Datasets](#datasets)
- [Awesome Text-to-Image/3D and RLHF](#awesome-text-to-image3d-and-rlhf)
  - [Text-to-Image Generation](#text-to-image-generation)
  - [Text-to-3D & RLHF](#text-to-3d--rlhf)
  - [Evaluation Metrics](#evaluation-metrics)
  - [Scene Synthesis and Interaction](#scene-synthesis-and-interaction)


## Awesome 3D Reconstruction

### Neural Radiance Fields
Papers focusing on neural radiance fields (NeRF) for view synthesis and scene representation.

- **[NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis](http://arxiv.org/abs/2003.08934)**  
  Ben Mildenhall, Pratul P. Srinivasan, Matthew Tancik, Jonathan T. Barron, Ravi Ramamoorthi, Ren Ng (2020)  
  Introduces NeRF, a method for synthesizing novel views of complex scenes using a continuous volumetric scene function optimized with sparse input views.

- **[Volume Rendering of Neural Implicit Surfaces](http://arxiv.org/abs/2106.12052)**  
  Lior Yariv, Jiatao Gu, Yoni Kasten, Yaron Lipman (2021)  
  Enhances neural volume rendering by modeling volume density as a function of geometry, improving reconstruction quality and enabling shape-appearance disentanglement.

### Signed Distance Functions
Research on learning continuous signed distance functions (SDFs) for shape representation.

- **[DeepSDF: Learning Continuous Signed Distance Functions for Shape Representation](http://arxiv.org/abs/1901.05103)**  
  Jeong Joon Park, Peter Florence, Julian Straub, Richard Newcombe, Steven Lovegrove (2019)  
  Presents DeepSDF, a learned SDF representation for high-quality shape interpolation and completion from partial 3D data, outperforming prior methods in model size and performance.

### Neural Implicit Surfaces
Advances in neural implicit surface reconstruction for multi-view 3D scenes.

- **[NeuS: Learning Neural Implicit Surfaces by Volume Rendering for Multi-View Reconstruction](http://arxiv.org/abs/2106.10689)**  
  Peng Wang, Lingjie Liu, Yuan Liu, Christian Theobalt, Taku Komura, Wenping Wang (2023)  
  Proposes NeuS, a neural surface reconstruction method using SDFs and a bias-free volume rendering formulation, achieving high-fidelity results without mask supervision.

### Monocular Geometric Reconstruction
Explorations of monocular cues for improving neural implicit surface reconstruction.

- **[MonoSDF: Exploring Monocular Geometric Cues for Neural Implicit Surface Reconstruction](http://arxiv.org/abs/2206.00665)**  
  Zehao Yu, Songyou Peng, Michael Niemeyer, Torsten Sattler, Andreas Geiger (2022)  
  Demonstrates that monocular depth and normal cues enhance reconstruction quality and speed, improving performance across single-object and multi-object scenes.

### Visual Geometry Transformers
Transformer-based approaches for unified 3D scene understanding.

- **[VGGT: Visual Geometry Grounded Transformer](https://github.com/facebookresearch/vggt)**  
  Jianyuan Wang, Minghao Chen, Nikita Karaev, Andrea Vedaldi, Christian Rupprecht, David Novotny (No date)  
  Introduces VGGT, a feed-forward network inferring 3D attributes like camera parameters and depth maps from sparse views, excelling in multiple 3D tasks.

### Indoor Compositional Reconstruction
Methods addressing challenges in reconstructing indoor scenes with partial observations.

- **[RICO: Regularizing the Unobservable for Indoor Compositional Reconstruction](http://arxiv.org/abs/2303.08605)**  
  Zizhang Li, Xiaoyang Lyu, Yuanyuan Ding, Mengmeng Wang, Yiyi Liao, Yong Liu (2023)  
  Proposes RICO, which regularizes occluded background geometry to improve object reconstruction in indoor scenes, enhancing compositional disentanglement.


## Awesome 3D Scene Generation

### 3D Scene Generation

This section includes papers that advance the field of 3D scene synthesis, focusing on geometric reasoning, layout planning, and generative models for creating realistic indoor environments.

1. **FirePlace: Geometric Refinements of LLM Common Sense Reasoning for 3D Object Placement**  
   - **Authors**: Huang et al.  
   - **Summary**: Introduces FirePlace, a framework that enhances Multimodal Large Language Models (MLLMs) for 3D object placement by combining geometric reasoning with common-sense understanding. It extracts geometric details, constructs constraints, and prunes placements for realistic scene generation, outperforming prior methods in complex scenes.  
   - **Link**: [arXiv:2503.04919](http://arxiv.org/abs/2503.04919)

2. **LayoutGPT: Compositional Visual Planning and Generation with Large Language Models**  
   - **Authors**: Feng et al.  
   - **Summary**: Proposes LayoutGPT, which leverages LLMs to generate plausible layouts from text inputs across 2D and 3D domains. By composing in-context visual demonstrations, it excels in handling numerical and spatial relations, achieving performance comparable to human-designed layouts.  
   - **Link**: [arXiv:2305.15393](http://arxiv.org/abs/2305.15393)

3. **DiffuScene: Denoising Diffusion Models for Generative Indoor Scene Synthesis**  
   - **Authors**: Tang et al.  
   - **Summary**: Presents DiffuScene, a diffusion-based model for indoor 3D scene synthesis. It generates unordered object sets with attributes like location and semantics, using shape feature diffusion for natural placements. The method supports applications like scene completion and text-conditioned synthesis.  
   - **Link**: [arXiv:2303.14207](http://arxiv.org/abs/2303.14207)


4. **I-Design: Personalized LLM Interior Designer**  
   - **Authors**: Çelen et al.  
   - **Summary**: Describes I-Design, a system that transforms user text inputs into feasible 3D interior designs via LLM agents. It generates scene graphs, optimizes object placements, and constructs 3D scenes, outperforming existing methods in quality and conceptual alignment with user goals.  
   - **Link**: [arXiv:2404.02838](http://arxiv.org/abs/2404.02838)
   
5. **OctoTools: An Agentic Framework with Extensible Tools for Complex Reasoning**  
   - **Authors**: Lu et al.  
   - **Summary**: Introduces OctoTools, a training-free, open-source framework that equips LLMs with tools for tasks like visual understanding and numerical reasoning. With standardized tool cards and a planner-executor system, it achieves significant accuracy gains over baselines like GPT-4o.  
   - **Link**: [arXiv:2502.11271](http://arxiv.org/abs/2502.11271)



## Awesome Visual Room Rearrangement

1. **PlanIT: Planning and Instantiating Indoor Scenes with Relation Graph and Spatial Prior Networks**  
   - Authors: Kai Wang, Yu-An Lin, Ben Weissmann, Manolis Savva, Angel X. Chang, Daniel Ritchie  
   - Year: 2019  
   - Summary: Introduces PlanIT, a framework that separates scene synthesis into planning (via relation graphs) and instantiation (via spatial prior networks), achieving high-quality indoor layouts with flexible graph-based representations.  
   - [arXiv: Not available](https://dl.acm.org/doi/10.1145/3306346.3322941)

2. **GRAINS: Generative Recursive Autoencoders for INdoor Scenes**  
   - Authors: Manyi Li, Akshay Gadi Patil, Kai Xu, Siddhartha Chaudhuri, Owais Khan, Ariel Shamir, Changhe Tu, Baoquan Chen, Daniel Cohen-Or, Hao Zhang  
   - Year: 2019  
   - Summary: Proposes GRAINS, a recursive neural network for generating hierarchical 3D indoor scenes, leveraging object grouping and spatial relations for diverse scene synthesis.  
   - [arXiv:1807.09193](http://arxiv.org/abs/1807.09193)

3. **Rearrangement: A Challenge for Embodied AI**  
   - Authors: Dhruv Batra, Angel X. Chang, Sonia Chernova, Andrew J. Davison, Jia Deng, Vladlen Koltun, Sergey Levine, Jitendra Malik, Igor Mordatch, Roozbeh Mottaghi, Manolis Savva, Hao Su  
   - Year: 2020  
   - Summary: Defines the rearrangement task as a benchmark for embodied AI, emphasizing the need for agents to restore object configurations in dynamic environments.  
   - [arXiv:2011.01975](http://arxiv.org/abs/2011.01975)

4. **Visual Room Rearrangement**  
   - Authors: Luca Weihs, Matt Deitke, Aniruddha Kembhavi, Roozbeh Mottaghi  
   - Year: 2021  
   - Summary: Presents the RoomR dataset with 6,000 rearrangement settings and demonstrates the complexity of navigation and object interaction, highlighting gaps in current embodied AI methods.  
   - [arXiv: Not available](https://ieeexplore.ieee.org/document/9578479/)

5. **Housekeep: Tidying Virtual Households Using Commonsense Reasoning**  
   - Authors: Yash Kant, Arun Ramachandran, Sriram Yenamandra, Igor Gilitschenski, Dhruv Batra, Andrew Szot, Harsh Agrawal  
   - Year: 2022  
   - Summary: Proposes a commonsense reasoning approach for household tidying, leveraging logical constraints to arrange objects in virtual environments.  
   - [arXiv: Not available](https://link.springer.com/10.1007/978-3-031-19842-7_21)

6. **Planning Large-scale Object Rearrangement Using Deep Reinforcement Learning**  
   - Authors: Sourav Ghosh, Dipanjan Das, Abhishek Agarwal, Marichi Chakraborty, Brojeshwar Bhowmick  
   - Year: 2022  
   - Summary: Introduces a deep RL method for large-scale rearrangement without explicit buffer spaces, demonstrating scalability across 2D and 3D scenarios.  
   - [arXiv: Not available](https://ieeexplore.ieee.org/document/9889793/)

7. **ConDor: Self-supervised Canonicalization of 3D Pose for Partial Shapes**  
   - Authors: Rahul Sajnani, Adrien Poulenard, Jivitesh Jain, Radhika Dua, Leonidas J. Guibas, Srinath Sridhar  
   - Year: 2022  
   - Summary: Develops ConDor, a self-supervised method for canonicalizing 3D poses of partial shapes, enhancing robustness in rearrangement tasks.  
   - [arXiv: Not available](https://ieeexplore.ieee.org/document/9878438/)

8. **A SIMPLE APPROACH FOR VISUAL ROOM REARRANGEMENT: 3D MAPPING AND SEMANTIC SEARCH**  
   - Authors: Brandon Trabucco, Gunnar A. Sigurdsson, Robinson Piramuthu, Gaurav S. Sukhatme, Ruslan Salakhutdinov  
   - Year: 2023  
   - Summary: Proposes a modular approach using semantic segmentation and 3D mapping, achieving a significant improvement in rearrangement accuracy (16.56% vs. 0.53%).  
   - [arXiv: Not available](https://ieeexplore.ieee.org/document/9878438/)

9. **Subtask Aware End-to-End Learning for Visual Room Rearrangement**  
   - Authors: Youngho Kim, Jong-Hwan Kim  
   - Year: 2023  
   - Summary: Introduces OSPNet and SAPNet for subtask-aware rearrangement, achieving high performance with fewer training steps via imitation learning.  
   - [arXiv: Not available](https://ieeexplore.ieee.org/document/10342320/)

10. **Task and Motion Planning with Large Language Models for Object Rearrangement**  
    - Authors: Yan Ding, Xiaohan Zhang, Chris Paxton, Shiqi Zhang  
    - Year: 2023  
    - Summary: Proposes LLM-GROP, using LLMs to extract commonsense knowledge for task and motion planning, generalizing to varying scene geometries.  
    - [arXiv: Not available](https://ieeexplore.ieee.org/document/10342169/)

11. **LEGO-Net: Learning Regular Rearrangements of Objects in Rooms**  
    - Authors: Qiuhong Anna Wei, Sijie Ding, Jeong Joon Park, Rahul Sajnani, Adrien Poulenard, Srinath Sridhar, Leonidas Guibas  
    - Year: 2023  
    - Summary: Presents LEGO-Net, a transformer-based method for regular rearrangements, introducing a metric for evaluating arrangement regularity.  
    - [arXiv: Not available](https://ieeexplore.ieee.org/document/10203922/)

12. **TidyBot: Personalized Robot Assistance with Large Language Models**  
    - Authors: Jimmy Wu, Rika Antonova, Adam Kan, Marion Lepert, Andy Zeng, Shuran Song, Jeannette Bohg, Szymon Rusinkiewicz, Thomas Funkhouser  
    - Year: 2023  
    - Summary: Demonstrates TidyBot, which uses LLMs for personalized tidying, achieving 91.2% accuracy on unseen objects and 85% in real-world tests.  
    - [arXiv:2305.05658](http://arxiv.org/abs/2305.05658)

13. **SceneScore: Learning a Cost Function for Object Arrangement**  
    - Authors: Ivan Kapelyukh, Edward Johns  
    - Year: 2023  
    - Summary: Introduces SceneScore, an energy-based model learning arrangement costs from images, enabling pose prediction and generalization to novel objects.  
    - [arXiv:2311.08530](http://arxiv.org/abs/2311.08530)

14. **ConSOR: A Context-aware Semantic Object Rearrangement Framework for Partially Arranged Scenes**  
    - Authors: Kartik Ramachandruni, Max Zuo, Sonia Chernova  
    - Year: 2023  
    - Summary: Proposes ConSOR, leveraging contextual cues from partially arranged scenes for rearrangement without explicit goal specifications.  
    - [arXiv:2310.00371](http://arxiv.org/abs/2310.00371)

15. **DALL-E-Bot: Introducing Web-Scale Diffusion Models to Robotics**  
    - Authors: Ivan Kapelyukh, Vitalis Vosylius, Edward Johns  
    - Year: 2023  
    - Summary: Integrates DALL-E for zero-shot rearrangement, inferring text descriptions and generating human-like arrangements.  
    - [arXiv:2210.02438](http://arxiv.org/abs/2210.02438)

16. **TarGF: Learning Target Gradient Field to Rearrange Objects Without Explicit Goal Specification**  
    - Authors: Mingdong Wu, Fangwei Zhong, Yulong Xia, Hao Dong  
    - Year: 2023  
    - Summary: Proposes TarGF, learning a gradient field from target distribution examples for efficient rearrangement without explicit goals.  
    - [arXiv:2209.00853](http://arxiv.org/abs/2209.00853)

17. **RealGraph: A Multiview Dataset for 4D Real-World Context Graph Generation**  
    - Authors: Haozhe Lin, Zequn Chen, Jinzhi Zhang, Bing Bai, Yu Wang, Ruqi Huang, Lu Fang  
    - Year: 2023  
    - Summary: Introduces RealGraph dataset and MCGNet for context graph generation, capturing 4D semantic relationships for rearrangement tasks.  
    - [arXiv: Not available](https://ieeexplore.ieee.org/document/10377352/)

18. **TASK PLANNING FOR VISUAL ROOM REARRANGEMENT UNDER PARTIAL OBSERVABILITY**  
    - Authors: Karan Mirakhor, Sourav Ghosh, Dipanjan Das, Brojeshwar Bhowmick  
    - Year: 2024  
    - Summary: Presents a modular planner with a novel search network and deep RL, outperforming prior methods in handling partial observability.  
    - [arXiv: Not available](https://ieeexplore.ieee.org/document/10377352/)

19. **LLM-Enhanced Scene Graph Learning for Household Rearrangement**  
    - Authors: Wenhao Li, Zhiyuan Yu, Qijin She, Zhinan Yu, Yuqing Lan, Chenyang Zhu, Ruizhen Hu, Kai Xu  
    - Year: 2024  
    - Summary: Enhances scene graphs with LLMs for household rearrangement, achieving state-of-the-art misplacement detection and planning.  
    - [arXiv:2408.12093](http://arxiv.org/abs/2408.12093)

20. **Efficient Object Rearrangement via Multi-view Fusion**  
    - Authors: Dehao Huang, Chao Tang, Hong Zhang  
    - Year: 2024  
    - Summary: Introduces a multi-view fusion system for efficient rearrangement, reducing redundant manipulations via accurate pose estimation.  
    - [arXiv: Not available](https://ieeexplore.ieee.org/document/10611213/)

21. **Dream2Real: Zero-Shot 3D Object Rearrangement with Vision-Language Models**  
    - Authors: Ivan Kapelyukh, Yifei Ren, Ignacio Alzugaray, Edward Johns  
    - Year: 2024  
    - Summary: Proposes Dream2Real, enabling zero-shot 3D rearrangement using vision-language models, robust to distractors and complex relations.  
    - [arXiv: Not available](https://ieeexplore.ieee.org/document/10611220/)

22. **Everyday Objects Rearrangement in a Human-like Manner via Robotic Imagination and Learning from Demonstration**  
    - Authors: Alberto Mendez, Adrian Prados, Elisabeth Menendez, Ramon Barber  
    - Year: 2024  
    - Summary: Combines zero-shot deep learning, diffusion models, and learning from demonstration for human-like 2D rearrangement.  
    - [arXiv: Not available](https://ieeexplore.ieee.org/document/10583854/)

23. **Lay-a-Scene: Personalized 3D Object Arrangement Using Text-to-Image Priors**  
    - Authors: Ohad Rahamim, Hilit Segev, Idan Achituve, Yuval Atzmon, Yoni Kasten, Gal Chechik  
    - Year: 2024  
    - Summary: Introduces Lay-a-Scene, using text-to-image priors for personalized 3D arrangements, inferring poses from 2D images.  
    - [arXiv:2406.00687](http://arxiv.org/abs/2406.00687)

24. **LVDiffusor: Distilling Functional Rearrangement Priors from Large Models into Diffusor**  
    - Authors: Yiming Zeng, Mingdong Wu, Long Yang, Jiyao Zhang, Hao Ding, Hui Cheng, Hao Dong  
    - Year: 2024  
    - Summary: Distills LLM and VLM priors into a diffusion model for functional rearrangement, outperforming baselines in compatibility.  
    - [arXiv:2312.01474](http://arxiv.org/abs/2312.01474)

### Datasets

- **RoomR (2021)**: Contains 6,000 rearrangement settings with 72 object types across 120 scenes, designed for evaluating navigation and interaction in rearrangement tasks. [Reference: Weihs et al., 2021]
- **RoPOR (2024)**: A benchmark dataset for rearrangement under partial observability, focusing on object search and rearrangement efficiency. [Reference: Mirakhor et al., 2024]
- **RealGraph (2023)**: A 4D multiview dataset for context graph generation, providing synchronized videos with annotated object relationships. [Reference: Lin et al., 2023]



## Awesome Text-to-Image/3D and RLHF

### Text-to-Image Generation

1. **Rich Human Feedback for Text-to-Image Generation**  
   *Authors*: Youwei Liang et al.  
   *Summary*: Introduces a dataset (RichHF-18K) with detailed human feedback to improve text-to-image models by addressing artifacts, misalignment, and aesthetic issues. The feedback is used to train a multimodal transformer, enhancing model finetuning and inpainting problematic regions.  
   *arXiv*: [2312.10240](http://arxiv.org/abs/2312.10240)

2. **Aligning Text-to-Image Models Using Human Feedback**  
   *Authors*: Kimin Lee et al.  
   *Summary*: Proposes a three-stage fine-tuning method using human feedback to improve text-to-image alignment, achieving better accuracy in generating objects with specified attributes compared to pre-trained models.  
   *arXiv*: [2302.12192](http://arxiv.org/abs/2302.12192)

3. **ImageReward: Learning and Evaluating Human Preferences for Text-to-Image Generation**  
   *Authors*: Jiazheng Xu et al.  
   *Summary*: Presents ImageReward, a human preference reward model trained on 137k expert comparisons, outperforming existing metrics and enabling reward feedback learning (ReFL) to optimize diffusion models.  
   *arXiv*: https://arxiv.org/abs/2304.05977

4. **Using Human Feedback to Fine-tune Diffusion Models without Any Reward Model**  
   *Authors*: Kai Yang et al.  
   *Summary*: Introduces D3PO, a direct preference optimization method for diffusion models that bypasses reward model training, achieving cost-effective fine-tuning with comparable results to reward-based methods.  
   *arXiv*: [CVPR 2024](http://arxiv.org/abs/2403.18422).

5. **Aligning Text-to-Image Diffusion Models with Reward Backpropagation**  
   *Authors*: Mihir Prabhudesai et al.  
   *Summary*: Proposes AlignProp, a method using end-to-end reward gradient backpropagation to align diffusion models, achieving higher rewards in fewer steps with improved simplicity.  
   *arXiv*: [2310.03739](http://arxiv.org/abs/2310.03739)

6. **Multimodal Large Language Model is a Human-Aligned Annotator for Text-to-Image Generation**  
   *Authors*: Xun Wu et al.  
   *Summary*: Introduces VisionPrefer, a preference dataset leveraging multimodal LLMs to evaluate text-to-image models across prompt-following, aesthetic, fidelity, and harmlessness, improving alignment via AI-generated synthetic data.  
   *arXiv*: [2404.15100](http://arxiv.org/abs/2404.15100)

### Text-to-3D & RLHF

7. **DreamReward: Text-to-3D Generation with Human Preference**  
   *Authors*: Junliang Ye et al.  
   *Summary*: Presents Reward3D, a human preference reward model for text-to-3D generation, paired with DreamFL, a tuning algorithm that optimizes multi-view diffusion models for high-fidelity 3D content.  
   *arXiv*: [2403.14613](http://arxiv.org/abs/2403.14613)

8. **DreamDPO: Aligning Text-to-3D Generation with Human Preferences via Direct Preference Optimization**  
   *Authors*: Zhenglin Zhou et al.  
   *Summary*: Proposes DreamDPO, a framework for optimizing text-to-3D generation using pairwise human preference comparisons, offering improved quality and controllability.  
   *arXiv*: [2502.04370](http://arxiv.org/abs/2502.04370)

9. **DreamScene: 3D Gaussian-based Text-to-3D Scene Generation via Formation Pattern Sampling**  
   *Authors*: Haoran Li et al.  
   *Summary*: Introduces DreamScene, a framework using Formation Pattern Sampling and progressive camera sampling to generate high-quality, consistent 3D scenes with flexible editing capabilities.  
   *arXiv*: [2404.03575](http://arxiv.org/abs/2404.03575)

10. **SceneTeller: Language-to-3D Scene Generation**  
    *Authors*: Başak Melis Öcal et al.  
    *Summary*: Proposes a text-based 3D room design pipeline using in-context learning and CAD model retrieval, enabling novices to create high-quality 3D scenes with style adjustments.  
    *arXiv*:  [ECCV 2024](http://arxiv.org/abs/2408.09958).

11. **3D-SceneDreamer: Text-driven 3D-consistent Scene Generation**  
    *Authors*: Songchun Zhang et al.  
    *Summary*: Employs a tri-plane NeRF and generative refinement network to synthesize 3D-consistent scenes, addressing limitations in outdoor and unreal scenarios.  
    *arXiv*:  [CVPR 2024](http://arxiv.org/abs/2403.10953).

### Evaluation Metrics

12. **Evaluating Text-to-Visual Generation with Image-to-Text Generation**  
    *Authors*: Zhiqiu Lin et al.  
    *Summary*: Introduces VQAScore, a visual-question-answering-based metric for evaluating text-to-visual alignment, outperforming traditional metrics across multiple benchmarks.  
    *arXiv*: [2404.01291](http://arxiv.org/abs/2404.01291)

13. **LLMScore: Unveiling the Power of Large Language Models in Text-to-Image Synthesis Evaluation**  
    *Authors*: Yujie Lu et al.  
    *Summary*: Proposes LLMScore, a framework using LLMs to evaluate text-to-image synthesis with multi-granularity compositionality, achieving higher correlation with human judgments than CLIP and BLIP.  
    *arXiv*: [2305.11116](http://arxiv.org/abs/2305.11116)

14. **GPT-4V(ision) is a Human-Aligned Evaluator for Text-to-3D Generation**  
    *Authors*: Tong Wu et al.  
    *Summary*: Uses GPT-4V to generate evaluation prompts and compare 3D assets, achieving human-aligned results across multiple criteria via Elo ratings.  
    *arXiv*: [2401.04092](http://arxiv.org/abs/2401.04092)

### Scene Synthesis and Interaction

15. **LayoutGPT: Compositional Visual Planning and Generation with Large Language Models**  
    *Authors*: Weixi Feng et al.  
    *Summary*: Proposes LayoutGPT, enhancing LLMs’ visual planning skills to generate plausible layouts for 2D and 3D scenes, improving text-to-image generation accuracy for numerical and spatial relations.  
    *arXiv*: [2305.15393](http://arxiv.org/abs/2305.15393)

16. **PhyScene: Physically Interactable 3D Scene Synthesis for Embodied AI**  
    *Authors*: Yandan Yang et al.  
    *Summary*: Introduces PhyScene, a method for generating interactive 3D scenes with realistic layouts and articulated objects, using physics-based guidance for embodied AI applications.  
    *arXiv*: [2404.09465](http://arxiv.org/abs/2404.09465)

17. **MOVIS: Enhancing Multi-Object Novel View Synthesis for Indoor Scenes**  
    *Authors*: Ruijie Lu et al.  
    *Summary*: Proposes MOVIS, enhancing multi-object novel view synthesis with structure-aware features and auxiliary tasks, improving cross-view consistency for indoor scenes.  
    *arXiv*: [2412.11457](http://arxiv.org/abs/2412.11457)

18. **ShapeLLM: Universal 3D Object Understanding for Embodied Interaction**  
    *Authors*: Zekun Qi et al.  
    *Summary*: Presents ShapeLLM, a 3D multimodal LLM for embodied interaction, using an enhanced ReCon++ encoder for superior geometry understanding and 3D interaction tasks.  
    *arXiv*: [2402.17766](http://arxiv.org/abs/2402.17766)

19. **RDT-1B: A Diffusion Foundation Model for Bimanual Manipulation**  
    *Authors*: Songming Liu et al.  
    *Summary*: Introduces RDT, a diffusion model for bimanual manipulation, leveraging a unified action space to enable transferrable physical knowledge for robotic tasks.  
    *arXiv*: [2410.07864](http://arxiv.org/abs/2410.07864)

