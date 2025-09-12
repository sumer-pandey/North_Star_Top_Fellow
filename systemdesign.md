# System Design — North Star

## Architecture
- **Client Layer:** PWA (React/Next.js), FCM push, offline mode
- **Edge Delivery:** AWS CloudFront, Route53, MediaConvert (HLS, captions, ABR for India 4G)
- **Auth:** AWS Cognito, OTP (Gupshup/Kaleyra)
- **API Gateway:** Kong (Mumbai region)

## Core Services
- User, Catalog (with OpenSearch), ROI (FastAPI + Redis), Roadmap Engine (Neo4j + FastAPI), Learning, Assessment, Project, Certificate, Payments (Razorpay/UPI), Notifications (WA/FCM), Experiments

## Data & ML
- Postgres, Redis, Neo4j, OpenSearch, Kafka/Kinesis, Redshift/Snowflake
- dbt, Airflow, SageMaker/Faiss

## Security & Observability
- OpenTelemetry → Jaeger; Prometheus, Grafana, Sentry
- AWS KMS, Secrets Manager, VPC isolation
- DPDP compliance (India data residency)

## Journey Alignment
- Acquire → Onboard → Roadmap → Pay → Starter Plan → Focus → Quiz/Project → Certificate → Share

📌 *Design aligned with AWS India infra & DPDP (Digital Personal Data Protection Act, 2023).*
