# MLE Transition Plan: SSE → Applied MLE (3 Months)

> Goal: Transition from Senior Software Engineer (Java/SpringBoot) to Applied Machine Learning Engineer
> Timeline: 3 months (~12 hrs/week, ~150 hours total)
> Target Role: Applied MLE (e.g., Waymo, similar production-focused ML roles)

---

## Gap Analysis

### Strengths to Leverage
- **Advanced Python** — biggest language barrier already cleared
- **Production engineering** (CI/CD, monitoring, reliability) → maps directly to MLOps
- **System design** skills translate well to ML system design
- **API/microservice experience** is valuable for model serving

### Critical Gaps to Fill
- ML algorithms and theory (supervised, unsupervised, evaluation metrics)
- Deep learning fundamentals and PyTorch
- Math refresher (linear algebra for neural nets, probability for ML theory)
- Data science toolkit (NumPy, Pandas, scikit-learn)
- End-to-end ML project experience (from data to production model)
- ML-specific system design patterns

---

## Month 1: ML Foundations (Weeks 1-4, ~50 hrs)

### Week 1-2: Math Refresher + Data Science Toolkit (24 hrs)

| Day | Topic | Resource | Time |
|-----|-------|----------|------|
| Mon/Wed/Fri | Linear Algebra: vectors, matrices, eigenvalues, SVD | 3Blue1Brown "Essence of Linear Algebra" (YouTube, free) | 1.5h/day |
| Tue/Thu | Probability & Statistics: distributions, Bayes, MLE/MAP | StatQuest (YouTube, free) | 1.5h/day |
| Sat | Hands-on: NumPy + Pandas exercises | Kaggle Learn (free) | 3h |
| Sun | Practice: implement matrix operations from scratch in Python | Self-practice | 2h |

**Deliverable:** NumPy 手写矩阵分解，熟练使用 Pandas 做数据清洗

### Week 3-4: ML Fundamentals (26 hrs)

| Day | Topic | Resource | Time |
|-----|-------|----------|------|
| Mon-Fri | Core ML: regression, classification, trees, SVM, clustering, evaluation metrics, bias-variance tradeoff, cross-validation | Andrew Ng — ML Specialization (Coursera) Course 1 & 2 | 2h/day |
| Sat | Hands-on: Kaggle competition (Titanic or Housing Prices) using scikit-learn | Kaggle | 3h |
| Sun | Review + write blog-style notes summarizing the week | Self-practice | 2h |

**Deliverable:** 完成 1 个 Kaggle 入门 competition，用 scikit-learn 完整跑通 train/evaluate/tune pipeline

---

## Month 2: Deep Learning & PyTorch (Weeks 5-8, ~50 hrs)

### Week 5-6: Neural Networks + PyTorch (24 hrs)

| Day | Topic | Resource | Time |
|-----|-------|----------|------|
| Mon/Wed | Neural network fundamentals: forward/backward prop, activation functions, loss functions, optimizers | fast.ai "Practical Deep Learning" Part 1 (Lessons 1-4) | 2h/day |
| Tue/Thu | PyTorch hands-on: tensors, autograd, nn.Module, DataLoader, training loop | PyTorch official tutorials | 2h/day |
| Sat | Project: implement a simple NN from scratch (MNIST classifier), then replicate in PyTorch | Self-practice | 3h |
| Sun | Review + compare PyTorch training loop patterns | Self-practice | 2h |

**Deliverable:** 从零手写一个 MNIST classifier (raw Python + NumPy)，然后用 PyTorch 重写

### Week 7-8: Key Architectures (26 hrs)

| Day | Topic | Resource | Time |
|-----|-------|----------|------|
| Mon/Wed | CNNs: convolutions, pooling, ResNet, transfer learning | fast.ai Part 1 (Lessons 5-7) + Stanford CS231n notes | 2h/day |
| Tue/Thu | Sequence models + Transformers: RNN, LSTM, attention, self-attention | "Attention Is All You Need" paper + Jay Alammar's illustrated guides | 2h/day |
| Sat | Project: fine-tune a pretrained model (ResNet/BERT) on a custom dataset | Hugging Face tutorials | 3h |
| Sun | Deep dive: read and annotate 1 ML paper related to your project | Self-practice | 2h |

**Deliverable:** 完成一个 transfer learning 项目 (fine-tune pretrained model)，能解释 Transformer 架构的每一层

---

## Month 3: Production ML & Portfolio (Weeks 9-12, ~50 hrs)

### Week 9-10: ML Infrastructure & MLOps (24 hrs)

| Day | Topic | Resource | Time |
|-----|-------|----------|------|
| Mon/Wed | ML system design patterns: training pipelines, feature stores, model serving, A/B testing, monitoring | "Designing Machine Learning Systems" by Chip Huyen (Chapters 1-6) | 2h/day |
| Tue/Thu | Hands-on MLOps: experiment tracking (MLflow/W&B), model registry, containerized serving | MLflow + Docker tutorials | 2h/day |
| Sat | Study ML system design cases: recommendation system, fraud detection, search ranking | ML System Design Interview resources | 3h |
| Sun | Practice: draw and explain an end-to-end ML system for a real product | Self-practice | 2h |

**Deliverable:** 能画出 end-to-end ML system 架构图，熟悉 MLflow experiment tracking

### Week 11-12: Portfolio Project + Interview Prep (26 hrs)

| Day | Topic | Resource | Time |
|-----|-------|----------|------|
| Mon-Fri | Build portfolio project: end-to-end ML pipeline (data processing → training → evaluation → serving API) | Self-directed project | 2h/day |
| Sat | ML coding practice: implement ML algorithms from scratch (logistic regression, decision tree, k-means) | LeetCode ML tag + self-practice | 3h |
| Sun | Mock ML system design interview practice | Chip Huyen's book + online resources | 2h |

**Deliverable:** 一个完整的 GitHub portfolio project，包含 data pipeline, model training, evaluation, REST API serving

---

## Portfolio Project Recommendation

针对 Applied MLE 岗位，建议做一个 **Autonomous Driving Object Detection Pipeline**，用 KITTI 或 nuScenes 数据集构建端到端目标检测 pipeline，直接对标 Waymo 的工作内容。

项目应覆盖以下环节：
1. **Data Ingestion** — 数据获取和预处理
2. **Feature Engineering** — 数据增强、标注处理
3. **Model Training** — PyTorch 训练循环 + experiment tracking (W&B/MLflow)
4. **Evaluation** — 多维度评估指标 (mAP, precision, recall)
5. **Model Serving** — FastAPI REST API 封装
6. **Monitoring** — 推理性能监控和日志

---

## Key Resources

| Category | Resource | Cost | Priority |
|----------|----------|------|----------|
| ML Fundamentals | Andrew Ng's ML Specialization (Coursera) | Free to audit | P0 |
| Deep Learning | fast.ai Practical Deep Learning | Free | P0 |
| PyTorch | PyTorch Official Tutorials | Free | P0 |
| Math | 3Blue1Brown + StatQuest (YouTube) | Free | P0 |
| ML System Design | "Designing ML Systems" by Chip Huyen | ~$40 | P0 |
| Transformers | Jay Alammar's Illustrated Guides | Free | P1 |
| Practice | Kaggle Competitions | Free | P1 |
| Experiment Tracking | W&B / MLflow docs | Free | P1 |
| Interview Prep | "ML System Design Interview" by A. Xu | ~$40 | P2 |

---

## Strategic Advice

1. **Leverage your SWE strengths** — 生产系统经验是很多 ML researcher 缺乏的。面试中强调你能把 model 从 notebook 带到 production。

2. **Focus on PyTorch, not TensorFlow** — 行业趋势明确偏向 PyTorch，所有目标 JD 都提到了 PyTorch。

3. **Build in public** — 把学习笔记和项目放在 GitHub 上，这是最有说服力的证明。

4. **Realistic target** — Waymo-style Applied MLE 是最现实的跳板，因为它重视工程能力 + ML 技能的结合。Netflix ML Scientist (L5) 需要研究背景和论文发表，3 个月内不太现实。

5. **Current job leverage** — 在 Walmart 的工作中，主动争取 AI/ML integration 相关的任务（JD 里提到了这部分），积累实战经验。

---

## Reference JDs

- [Google SSE ML, Core ML](Jobs/01_Google_SSE_ML.md) — ML Infra, training frameworks, $174K-$252K
- [Walmart SSE (Current)](Jobs/02_walmart_SSE.md) — Java/SpringBoot, API, $117K-$234K
- [Waymo Senior MLE, Simulation](Jobs/03_Waymo_Senior%20Machine%20Learning%20Engineer%2C%20Simulation.md) — Production ML, Python/C++, $204K-$259K
- [Netflix ML Scientist L4/L5](Jobs/04_Netflix_MLS.md) — LLMs, multi-modal, $466K-$750K
