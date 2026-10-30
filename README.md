🐔 Chicken Health Monitoring System — 21-Day Roadmap

Goal: Build a backend system that monitors chicken farm conditions using Raspberry Pi sensors, MQTT, ASP.NET Core, SQL Server, SignalR, and Twilio.

Duration: 3 Weeks · 21 Days

Daily commitment: 2–3 hours

---

Week 1 — C# & ASP.NET Core Fundamentals

Goal: Understand the backend architecture and build a basic REST API connected to SQL Server.

Day 1 — C# Revision

- [ ] Review OOP concepts: Classes, Objects, Inheritance, Interfaces.
- [ ] Practice Collections, Lists, and Dictionaries.
- [ ] Review LINQ, Async/Await, and Exception Handling.

Day 2 — HTTP & REST APIs

- [ ] Understand HTTP methods: GET, POST, PUT, DELETE.
- [ ] Understand Status Codes and JSON.
- [ ] Learn REST API principles.

Resources: "HTTP overview" (https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview)

Day 3 — ASP.NET Core Introduction

- [ ] Understand ASP.NET Core project structure.
- [ ] Learn Controllers and Routing.
- [ ] Understand Dependency Injection.
- [ ] Create your first Web API.

Resources: "ASP.NET Core Web API Fundamentals" (https://learn.microsoft.com/en-us/aspnet/core/web-api/)

Day 4 — SQL & Database Fundamentals

- [ ] Understand relational databases.
- [ ] Review Tables, Primary Keys, and Foreign Keys.
- [ ] Practice SELECT, INSERT, UPDATE, DELETE.
- [ ] Understand basic JOIN operations.

Resources: "Database Fundamentals Video" (https://youtu.be/pPqazMTzNOM?si=OaCJE6MRs26bOIL1)

Day 5 — Entity Framework Core

- [ ] Understand ORM and EF Core.
- [ ] Learn DbContext and DbSet.
- [ ] Create Models.
- [ ] Practice Migrations.
- [ ] Connect ASP.NET Core to SQL Server.

Resources: "EF Core Documentation" (https://learn.microsoft.com/en-us/ef/core/)

Day 6 — Database Design

- [ ] Design the SensorReadings table.
- [ ] Design the Devices table.
- [ ] Design the Alerts table.
- [ ] Define relationships between tables.

Day 7 — Week 1 Practical Task

- [ ] Create an ASP.NET Core Web API.
- [ ] Connect it to SQL Server using EF Core.
- [ ] Implement CRUD operations for SensorReadings.
- [ ] Test endpoints using Postman.

Week 1 Deliverable: Working REST API connected to SQL Server.

---

Week 2 — MQTT & Real-Time Data

Goal: Receive sensor data through MQTT, process it in the backend, and display updates in real time.

Day 8 — MQTT Fundamentals

- [ ] Understand MQTT architecture.
- [ ] Learn Publisher and Subscriber.
- [ ] Understand Broker, Topics, and Payloads.
- [ ] Learn QoS levels.

Resources: "MQTT Introduction Video" (https://youtu.be/l_CT1sGgvdk?si=FurV_MHEUnGFMat9)

Day 9 — MQTT Broker

- [ ] Understand MQTT Broker responsibilities.
- [ ] Install Mosquitto.
- [ ] Publish test messages.
- [ ] Subscribe to MQTT topics.

Resources: "Mosquitto Documentation" (https://mosquitto.org/documentation/)

Day 10 — MQTTnet

- [ ] Install MQTTnet in the ASP.NET Core project.
- [ ] Create an MQTT client.
- [ ] Connect to the Broker.
- [ ] Subscribe to sensor topics.
- [ ] Receive incoming messages.

Resources: "MQTTnet GitHub" (https://github.com/dotnet/MQTTnet)

Day 11 — Background Services

- [ ] Understand BackgroundService.
- [ ] Learn IHostedService.
- [ ] Run MQTT subscription as a background service.
- [ ] Handle connection and disconnection.

Resources: "Hosted Services in ASP.NET Core" (https://learn.microsoft.com/en-us/aspnet/core/fundamentals/host/hosted-services)

Day 12 — Process & Store Sensor Data

- [ ] Define the sensor JSON payload.
- [ ] Deserialize incoming MQTT messages.
- [ ] Validate temperature, humidity, and ammonia values.
- [ ] Save valid readings to SQL Server.
- [ ] Handle invalid messages and errors.

Day 13 — SignalR

- [ ] Understand WebSockets and SignalR.
- [ ] Create a SignalR Hub.
- [ ] Send sensor updates to connected clients.
- [ ] Test real-time communication.

Resources: "ASP.NET Core SignalR" (https://learn.microsoft.com/en-us/aspnet/core/signalr/introduction)

Day 14 — Week 2 Integration Task

- [ ] Receive MQTT messages.
- [ ] Process and validate sensor data.
- [ ] Store readings in SQL Server.
- [ ] Broadcast updates using SignalR.

Week 2 Deliverable: Real-time sensor data pipeline working end to end.

---

Week 3 — Alerts, Security & Final Integration

Goal: Add authentication, alert notifications, testing, and complete the backend integration.

Day 15 — Authentication & Authorization

- [ ] Understand Authentication vs Authorization.
- [ ] Learn ASP.NET Core Identity basics.
- [ ] Understand JWT Authentication.
- [ ] Learn role-based authorization.

Resources:

- "Authentication & Authorization Playlist" (https://youtube.com/playlist?list=PLOeFnOV9YBa4yaz-uIiT5ZW3QQGHJQXi&si=pTCn45Zu_ITqqE6P)
- "ASP.NET Core Authentication" (https://learn.microsoft.com/en-us/aspnet/core/security/authentication/)

Day 16 — Twilio SMS

- [ ] Understand Twilio SMS API.
- [ ] Create a Twilio account.
- [ ] Configure credentials securely.
- [ ] Send a test SMS from ASP.NET Core.

Resources: "Twilio C# SMS Quickstart" (https://www.twilio.com/docs/messaging/quickstart/csharp-dotnet-core)

Day 17 — Alert Logic

- [ ] Define safe ranges for temperature, humidity, and ammonia.
- [ ] Detect abnormal readings.
- [ ] Create alert records in SQL Server.
- [ ] Send SMS notifications when thresholds are exceeded.
- [ ] Prevent repeated unnecessary notifications.

Day 18 — Security & Configuration

- [ ] Use appsettings and environment variables.
- [ ] Keep secrets out of source control.
- [ ] Validate incoming data.
- [ ] Handle exceptions and logging.
- [ ] Secure API endpoints.

Day 19 — Testing

- [ ] Test API endpoints using Postman.
- [ ] Test MQTT message handling.
- [ ] Test database operations.
- [ ] Test SignalR updates.
- [ ] Test SMS alert scenarios.

Day 20 — Full System Integration

- [ ] Connect Raspberry Pi / simulated sensor publisher.
- [ ] Connect MQTT Broker.
- [ ] Receive messages through MQTTnet.
- [ ] Store readings using EF Core.
- [ ] Broadcast updates using SignalR.
- [ ] Trigger alerts through Twilio.

Day 21 — Final Review

- [ ] Review project architecture.
- [ ] Fix bugs and improve error handling.
- [ ] Organize the project structure.
- [ ] Write README documentation.
- [ ] Add architecture diagram.
- [ ] Test the complete workflow.

Week 3 Deliverable: Complete backend integration with real-time monitoring and SMS alerts.

---

System Architecture

Raspberry Pi Sensors
        |
        v
    MQTT Broker
        |
        v
 MQTTnet Subscriber
        |
        v
 Data Validation
        |
        v
    SQL Server
        |
        +------> SignalR ------> Dashboard
        |
        +------> Alert Service
                       |
                       v
                   Twilio SMS

Final Project Checklist

- [ ] ASP.NET Core Web API
- [ ] SQL Server Database
- [ ] Entity Framework Core
- [ ] MQTT Broker
- [ ] MQTTnet Subscriber
- [ ] Background Service
- [ ] Sensor Data Validation
- [ ] SignalR Real-Time Updates
- [ ] Authentication & Authorization
- [ ] Twilio SMS Notifications
- [ ] Testing & Documentation

---

Important: Focus on understanding and implementing each part. Don't just watch tutorials — write code and test every feature.
