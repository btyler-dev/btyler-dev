## tyler bednar
*forward deployed engineer · ai/ml*


**I train, fine-tune and serve models, then make them fast.** For 10+ years I've taken machine learning from notebook to production: forecasting and recommendations first, then deep learning for NLP and computer vision, and today mostly open-weight LLMs, fine-tuned with LoRA, QLoRA and RLHF and served with vLLM and Triton. I own the MLOps around all of it, on AWS, Azure and GCP.


| 🧪 prototype | 🏋️ train | 📏 evaluate | 🚀 serve | 📡 monitor |
|:-:|:-:|:-:|:-:|:-:|
| notebook, baseline, eval set | distributed, tracked, reproducible | offline metrics, then A/B | batched, quantized, autoscaled | drift, latency, retrain triggers |


### what changes when I ship it


```diff
@@ loraloom · fine-tuning @@
- a one-off training script for every new domain model
+ one YAML spec → 4-bit QLoRA on Ray → eval gate → versioned adapter in MLflow


@@ servo · inference @@
- LLMs and classic deep learning models on separate stacks
+ vLLM and Triton behind one API, autoscaled on queue depth to a p95 latency budget


@@ shelfwatch · computer vision @@
- out-of-stocks and misplaced products spotted late
+ YOLO + EfficientNet on in-store edge devices, retrained from low-confidence frames


@@ cartmate · recommendations @@
- new ranking ideas shipped straight to full traffic
+ two-tower retrieval + XGBoost ranker, offline replay, then an A/B test


@@ storecast · forecasting @@
- one global error number
+ store × sku × day forecasts, reconciled to regions, backtested by segment


@@ formsight · document ai @@
- form fields keyed in by hand
+ layout-aware NER → schema-validated JSON, unsure fields routed to a reviewer
```


### toolbelt


<img src="https://skillicons.dev/icons?i=py,pytorch,tensorflow,sklearn,opencv,fastapi,redis,docker,kubernetes,terraform,githubactions,prometheus,grafana,aws,azure,gcp&perline=16" />


<sub>also: PEFT · DeepSpeed · Ray · vLLM · Triton · ONNX · YOLO · Hugging Face · LangGraph · MLflow · DVC · W&B · Airflow · dbt · Evidently · Spark</sub>

