# Kafka Rider Updates Application

This application demonstrates the use of Kafka to create, produce, and consume messages for a topic named `rider-updates`. The system consists of an admin for managing Kafka topics, a producer for sending rider updates, and a consumer for processing these updates.

---

## Table of Contents
- [Prerequisites](#prerequisites)
- [Project Structure](#project-structure)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
  - [Admin](#admin)
  - [Producer](#producer)
  - [Consumer](#consumer)
- [Example Workflow](#example-workflow)

---

## Prerequisites
1. **Kafka Installation**: Ensure Kafka is installed and running on your system. Set up the Kafka server and broker.
2. **Node.js**: Version 14+ recommended.
3. **KafkaJS**: Used as the Kafka client library in Node.js.

---

## Project Structure

Here’s the complete README.md file you can directly copy and paste into your project directory:

markdown
# Kafka Rider Updates Application

This application demonstrates the use of Kafka to create, produce, and consume messages for a topic named `rider-updates`. The system consists of an admin for managing Kafka topics, a producer for sending rider updates, and a consumer for processing these updates.

---

## Table of Contents
- [Prerequisites](#prerequisites)
- [Project Structure](#project-structure)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
  - [Admin](#admin)
  - [Producer](#producer)
  - [Consumer](#consumer)
- [Example Workflow](#example-workflow)

---

## Prerequisites
1. **Kafka Installation**: Ensure Kafka is installed and running on your system. Set up the Kafka server and broker.
2. **Node.js**: Version 14+ recommended.
3. **KafkaJS**: Used as the Kafka client library in Node.js.

---

## Project Structure
Kafka_app/ │ ├── client.js # Kafka client configuration ├── admin.js # Script to create and manage Kafka topics ├── producer.js # Producer script for sending rider updates ├── consumer.js # Consumer script for processing messages ├── package.json # Dependencies and scripts └── README.md # Documentation

---

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd Kafka_app
Install dependencies:


npm install
Update the Kafka broker address in client.js if necessary:

javascript
brokers: ["192.168.1.38:9092"], // Replace with your Kafka broker address
Start the Kafka server and broker.

Usage:

Admin
Run admin.js to create the rider-updates topic with 2 partitions:

bash
Copy code
node admin.js

Producer
Run producer.js to send rider updates:
node producer.js
You can then input rider updates in the following format:
<riderName> <location>
Example: John North will send an update for John in the North partition.

Consumer
Run consumer.js with a group ID to start consuming messages:
node consumer.js <group-id>
