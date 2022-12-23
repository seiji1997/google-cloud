# Google Cloud Certified Professional Machine Learning Engineer
I will take 2022/12/31. This is my final exam in 2022.

- [Official Professional Machine Learning Engineer](https://cloud.google.com/certification/guides/machine-learning-engineer)
- [How to study for (and pass) Google's Professional Machine Learning Engineer certification](https://www.linkedin.com/pulse/how-study-pass-googles-professional-machine-learning-engineer-siegel/)
- [Machine Learning Glossary](https://developers.google.com/machine-learning/glossary)

## LEARNING STEP
- 1, [Official Professional Machine Learning Engineer](https://cloud.google.com/certification/guides/machine-learning-engineer)
- 2, [Professional Machine Learning Engineer Sample Questions](https://docs.google.com/forms/d/e/1FAIpQLSeYmkCANE81qSBqLW0g2X7RoskBX9yGYQu-m1TtsjMvHabGqg/viewform)
- 3, [Google Cloud Machine Learning Engineer Certification Prep](https://www.udemy.com/course/google-cloud-machine-learning-engineer-certification-prep/)
- 4, [Google Cloud Professional Machine Learning Engineer *2022*](https://www.udemy.com/course/google-cloud-professional-machine-learning-engineer-2022/)
- 5, [REGISTER FOR AN EXAM](https://www.webassessor.com/googlecloudjp)

## LEARNING PATH
- [Data Engineering and Smart Analytics](https://cloud.google.com/training/data-engineering-and-analytics)
- [Machine Learning and AI](https://cloud.google.com/training/machinelearning-ai)


## MACHINE LEARNING ON GOOGLE
- [Best practices for implementing machine learning on Google Cloud](https://cloud.google.com/architecture/ml-on-gcp-best-practices)
- [Best practices for performance and cost optimization for machine learning](https://cloud.google.com/architecture/best-practices-for-ml-performance-cost)

## MACHINE LEARNING RESOURCES
- [Machine Learning Crash Course with TensorFlow APIs](https://developers.google.com/machine-learning/crash-course)
- [TensorFlow](https://www.tensorflow.org/)
- [Scikit-Learn](https://scikit-learn.org/stable/)
- [XGBoost](https://xgboost.readthedocs.io/en/stable/)
- [Security - MLOps](https://www.frontiersin.org/articles/10.3389/fdata.2020.587139/full)

## DATA ENGINEERING RESOURCES
- [Apache Beam](https://beam.apache.org/) - [Google Cloud Dataflow](https://cloud.google.com/dataflow)
- [Apache Spark](https://spark.apache.org/) - [Google Cloud Dataproc](https://cloud.google.com/dataproc)

## DATA SCIENCE
- [datasciencedojo](https://datasciencedojo.com/blog) 

## PAPER
- [Hidden Technical Debt in Machine Learning Systems](https://proceedings.neurips.cc/paper/2015/file/86df7dcfd896fcaf2674f757a2463eba-Paper.pdf)
- [exploratory_data_analysis_for_feature_selection_in_machine_learning.pdf](https://services.google.com/fh/files/misc/exploratory_data_analysis_for_feature_selection_in_machine_learning.pdf)

## MLOps
Machine Learning systems can be categorized in eight different categories: data collection, data processing, feature engineering, data labelling, model design, model training and optimization, endpoint deployment, and endpoint monitoring. Each step in the machine learning lifecycle is built in their own system, but requires interconnection. These are the minimum systems that enterprises need to scale machine learning within their organization.<br>

- Deployment and automation<br>
https://dagshub.com/blog/code-to-production-ready-machine-learning-in-4-steps/<br>
- Reproducibility of models and predictions<br>
https://petewarden.com/2018/03/19/the-machine-learning-reproducibility-crisis/<br>
- Diagnostics<br>
https://petewarden.com/2018/03/19/the-machine-learning-reproducibility-crisis/<br>
- Governance and regulatory compliance<br>
https://www.techtarget.com/searchdatamanagement/definition/data-governance<br>
- Scalability<br>
https://www.oreilly.com/radar/podcast/how-to-train-and-deploy-deep-learning-at-scale/<br>
- Collaboration<br>
https://www.iottechexpo.com/2017/10/ai/iot-machine-learning-ml-ai-why-collaboration-key/<br>
- Business uses<br>
https://www.mckinsey.com/featured-insights/digital-disruption/whats-now-and-next-in-analytics-ai-and-automation<br>
- Monitoring and management<br>
https://www.iguazio.com/blog/mlops-challenges-solutions-future-trends/<br>

### materials
- [wiki](https://en.wikipedia.org/wiki/MLOps)
- [“What is ML Ops? Best Practices for Devops for ML”. YouTube.](https://www.youtube.com/watch?v=_jnhXzY1HCw)
- [“Should every business function have an Ops extension?”. Tech HQ.](https://techhq.com/2018/04/should-every-business-function-have-an-ops-extension/)
- [“How to build AI culture: go through the curve of enlightenment”. Medium. Hackernoon.](https://hackernoon.com/how-to-build-ai-culture-go-through-the-curve-of-enlightenment-21c239c1d5a7)
- [“MLOps with serverless architectures (October 2018)”. LinkedIn SlideShare. Julien Simon.](https://www.slideshare.net/JulienSIMON5/mlops-with-serverless-architectures-october-2018)
- [“Operational Machine Learning: Seven Considerations for Successful MLOps”. KDNuggets.](https://www.kdnuggets.com/2018/04/operational-machine-learning-successful-mlops.html)
- [“BD Podcast Ep 34 – Putting AI to Work with MLOps Powered by ParallelM”. Big Data Beard.](https://bigdatabeard.com/bd-podcast-ep-34-putting-ai-to-work-with-mlops-powered-by-parallelm/)
- [“What is ML Ops? Solutions and best practices for applying DevOps to production ML services”. Artificial Intelligence Conference. O'Reilly.](https://conferences.oreilly.com/artificial-intelligence/ai-eu-2018/public/schedule/detail/68247.html)

## MUST UNDERSTAND CONCEPTS
### Section 1: Framing ML problems
1.1 Translating business challenges into ML use cases. Considerations include:

    ●  Choosing the best solution (ML vs. non-ML, custom vs. pre-packaged [e.g., AutoML, Vision API]) based on the business requirements 

    ●  Defining how the model output should be used to solve the business problem

    ●  Deciding how incorrect results should be handled

    ●  Identifying data sources (available vs. ideal)

1.2 Defining ML problems. Considerations include:

    ●  Problem type (e.g., classification, regression, clustering)

    ●  Outcome of model predictions

    ●  Input (features) and predicted output format

1.3 Defining business success criteria. Considerations include:

    ●  Alignment of ML success metrics to the business problem

    ●  Key results

    ●  Determining when a model is deemed unsuccessful

1.4 Identifying risks to feasibility of ML solutions. Considerations include: 

    ●  Assessing and communicating business impact

    ●  Assessing ML solution readiness

    ●  Assessing data readiness and potential limitations

    ●  Aligning with Google’s Responsible AI practices (e.g., different biases)
- []()
- []()

### Section 2: Architecting ML solutions
2.1 Designing reliable, scalable, and highly available ML solutions. Considerations include:

    ●  Choosing appropriate ML services for the use case (e.g., Cloud Build, Kubeflow)

    ●  Component types (e.g., data collection, data management)

    ●  Exploration/analysis

    ●  Feature engineering

    ●  Logging/management

    ●  Automation

    ●  Orchestration

    ●  Monitoring

    ●  Serving

2.2 Choosing appropriate Google Cloud hardware components. Considerations include:

    ●  Evaluation of compute and accelerator options (e.g., CPU, GPU, TPU, edge devices) 

2.3 Designing architecture that complies with security concerns across sectors/industries. 

Considerations include:

    ●  Building secure ML systems (e.g., protecting against unintentional exploitation of data/model, hacking)

    ●  Privacy implications of data usage and/or collection (e.g., handling sensitive data such as Personally Identifiable Information [PII] and Protected Health Information [PHI])
- []()
- []()
- []()

### Section 3: Designing data preparation and processing systems
3.1 Exploring data (EDA). Considerations include:

    ●  Visualization

    ●  Statistical fundamentals at scale

    ●  Evaluation of data quality and feasibility

    ●  Establishing data constraints (e.g., TFDV)

3.2 Building data pipelines. Considerations include:

    ●  Organizing and optimizing training datasets

    ●  Data validation

    ●  Handling missing data

    ●  Handling outliers

    ●  Data leakage

3.3 Creating input features (feature engineering). Considerations include:

    ●  Ensuring consistent data pre-processing between training and serving

    ●  Encoding structured data types

    ●  Feature selection

    ●  Class imbalance

    ●  Feature crosses

    ●  Transformations (TensorFlow Transform)
- []()
- []()
- []()

### Section 4: Developing ML models
4.1 Building models. Considerations include:

    ●  Choice of framework and model

    ●  Modeling techniques given interpretability requirements

    ●  Transfer learning

    ●  Data augmentation

    ●  Semi-supervised learning

    ●  Model generalization and strategies to handle overfitting and underfitting

4.2 Training models. Considerations include:

    ●  Ingestion of various file types into training (e.g., CSV, JSON, IMG, parquet or databases, Hadoop/Spark)

    ●  Training a model as a job in different environments

    ●  Hyperparameter tuning

    ●  Tracking metrics during training

    ●  Retraining/redeployment evaluation

4.3 Testing models. Considerations include:

    ●  Unit tests for model training and serving

    ●  Model performance against baselines, simpler models, and across the time dimension

    ●  Model explainability on Vertex AI

4.4 Scaling model training and serving. Considerations include:

    ●  Distributed training

    ●  Scaling prediction service (e.g., Vertex AI Prediction, containerized serving)
- [Vertex AI](https://cloud.google.com/vertex-ai)
- []()
- []()
- []()

### Section 5: Automating and orchestrating ML pipelines
5.1 Designing and implementing training pipelines. Considerations include:

    ●  Identification of components, parameters, triggers, and compute needs (e.g., Cloud Build, Cloud Run)

    ●  Orchestration framework (e.g., Kubeflow Pipelines/Vertex AI Pipelines, Cloud Composer/Apache Airflow)

    ●  Hybrid or multicloud strategies

    ●  System design with TFX components/Kubeflow DSL 

5.2 Implementing serving pipelines. Considerations include:

    ●  Serving (online, batch, caching)

    ●  Google Cloud serving options

    ●  Testing for target performance

    ●  Configuring trigger and pipeline schedules

5.3 Tracking and auditing metadata. Considerations include:

    ●  Organizing and tracking experiments and pipeline runs

    ●  Hooking into model and dataset versioning

    ●  Model/dataset lineage
- []()
- []()
- []()

### Section 6: Monitoring, optimizing, and maintaining ML solutions
6.1 Monitoring and troubleshooting ML solutions. Considerations include:

    ●  Performance and business quality of ML model predictions

    ●  Logging strategies

    ●  Establishing continuous evaluation metrics (e.g., evaluation of drift or bias)

    ●  Understanding Google Cloud permissions model

    ●  Identification of appropriate retraining policy

    ●  Common training and serving errors (TensorFlow)

    ●  ML model failure and resulting biases

6.2 Tuning performance of ML solutions for training and serving in production. 

Considerations include:

    ●  Optimization and simplification of input pipeline for training

    ●  Simplification techniques 
- []()
- []()
- []()
