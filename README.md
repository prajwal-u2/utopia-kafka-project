# Utopia – Real-Time Analytics Pipeline using Apache Kafka & Pinot

## Project Overview

This project implements a comprehensive real-time analytics pipeline for Utopia, a fictional e-commerce platform. The solution leverages Apache Kafka for stream processing and Apache Pinot for real-time analytics, providing insights into user behavior, sales performance, and system metrics.

## Project Phases

### Phase 1: Technology Evaluation
- **Document**: `Phase-1_RabbitMQ-vs-Kafka.pdf`
- **Focus**: Comparative analysis between RabbitMQ and Apache Kafka
- **Outcome**: Technology selection and architecture decisions

### Phase 2: System Design & Architecture
- **Document**: `Phase-2_Insights-Design.excalidraw`
- **Focus**: System architecture design and data flow diagrams
- **Outcome**: Detailed system design and component interactions

### Phase 3: Stream Processing Proof of Concept
- **Document**: `Phase-3_Stream-Processing-POC.pdf`
- **Focus**: Implementation of real-time stream processing using Apache Kafka
- **Outcome**: Working stream processing pipeline with data transformation

### Phase 4: OLAP Analytics with Apache Pinot
- **Document**: `Phase-4_Pinot-OLAP-POC.pdf`
- **Focus**: Real-time analytics and querying capabilities using Apache Pinot
- **Outcome**: Interactive dashboard and analytics platform

## Codebase Locations

The implementation code for this project is located in two separate repositories:

1. **data-demo**: Contains the core data pipeline implementation, Kafka producers/consumers, and data processing logic
2. **stream-processing-workshop**: Contains workshop materials, examples, and additional stream processing implementations

## Technology Stack

- **Apache Kafka**: Message streaming platform for real-time data ingestion
- **Apache Pinot**: Real-time distributed OLAP datastore
- **Apache Zookeeper**: Distributed coordination service
- **Docker**: Containerization for easy deployment
- **Java/Python**: Programming languages for stream processing applications

## Key Features

- Real-time data ingestion from multiple sources
- Stream processing with data transformation and enrichment
- Real-time analytics and querying capabilities
- Scalable and fault-tolerant architecture
- Interactive dashboards for business insights

## Getting Started

### Prerequisites

- Docker and Docker Compose
- Java 11 or higher
- Python 3.8 or higher
- Apache Kafka (can be run via Docker)
- Apache Pinot (can be run via Docker)

### Setup Instructions

1. Clone the repositories:
   ```bash
   git clone <data-demo-repo-url>
   git clone <stream-processing-workshop-repo-url>
   ```

2. Start the infrastructure services:
   ```bash
   # Start Kafka and Zookeeper
   docker-compose up -d kafka zookeeper
   
   # Start Apache Pinot
   docker-compose up -d pinot
   ```

3. Run the data pipeline:
   ```bash
   # Navigate to data-demo directory
   cd data-demo
   # Follow the setup instructions in the data-demo README
   ```

4. Access the analytics dashboard:
   - Pinot Query Console: http://localhost:9000
   - Pinot Data Explorer: http://localhost:9000/query

## Project Structure

```
utopia-kafka-project/
├── Phase-1_RabbitMQ-vs-Kafka.pdf          # Technology evaluation
├── Phase-2_Insights-Design.excalidraw     # System architecture design
├── Phase-3_Stream-Processing-POC.pdf      # Stream processing implementation
├── Phase-4_Pinot-OLAP-POC.pdf            # OLAP analytics implementation
└── README.md                             # This file
```

## Contributing

This project was developed as part of an academic course on Event-Driven Architecture and Stream Processing. For questions or contributions, please refer to the course guidelines.

## License

This project is for educational purposes. Please refer to the individual phase documents for specific implementation details and technical specifications.
