🐔 Chicken Health Monitoring System – Backend Roadmap

Duration: 21 Days

Week 1 – Backend & Database

Day 1 – C# Revision

- [ ] Classes, Objects, Interfaces, Inheritance
- [ ] Collections and LINQ
- [ ] Exception Handling
- [ ] Async/Await and Tasks

Day 2 – HTTP & REST APIs

- [ ] HTTP Methods and Status Codes
- [ ] JSON
- [ ] REST API Principles
- [ ] Controllers and Endpoints

Resource: "ASP.NET Core Web API" (https://learn.microsoft.com/en-us/aspnet/core/web-api/)

Day 3 – ASP.NET Core Basics

- [ ] Create a Web API Project
- [ ] Program.cs and Middleware
- [ ] Dependency Injection
- [ ] Services and Controllers

Resource: "ASP.NET Core Fundamentals" (https://learn.microsoft.com/en-us/aspnet/core/fundamentals/)

Day 4 – SQL & Database Fundamentals

- [ ] Tables and Relationships
- [ ] Primary Keys and Foreign Keys
- [ ] SELECT, INSERT, UPDATE, DELETE
- [ ] JOIN
- [ ] Database Design

Resources:

- "Database Fundamentals Course" (https://youtu.be/pPqazMTzNOM?si=OaCJE6MRs26bOIL1)
- "SQL Server Fundamentals" (https://learn.microsoft.com/en-us/sql/sql-server/)

Day 5 – Entity Framework Core

- [ ] ORM Concepts
- [ ] DbContext and Entities
- [ ] Relationships
- [ ] Migrations

Resource: "Entity Framework Core" (https://learn.microsoft.com/en-us/ef/core/)

Day 6 – Database Design

- [ ] Sensors Table
- [ ] SensorReadings Table
- [ ] Alerts Table
- [ ] Entity Relationships
- [ ] Connect SQL Server to ASP.NET Core

Day 7 – Practical Task

- [ ] Create Backend Project
- [ ] Implement Database Models
- [ ] Configure EF Core
- [ ] Create Sensor Readings APIs
- [ ] Test APIs using Postman

---

Week 2 – MQTT & Real-Time Communication

Day 8 – MQTT Fundamentals

- [ ] MQTT Broker, Publisher, Subscriber
- [ ] Topics
- [ ] QoS Levels
- [ ] Retained Messages and Last Will

Resources:

- "MQTT Tutorial" (https://youtu.be/l_CT1sGgvdk?si=FurV_MHEUnGFMat9)
- "MQTT Essentials" (https://www.hivemq.com/mqtt-essentials/)

Day 9 – MQTT Broker

- [ ] Install Mosquitto
- [ ] Publish Messages
- [ ] Subscribe to Topics
- [ ] Test MQTT Communication

Resource: "Mosquitto Documentation" (https://mosquitto.org/documentation/)

Day 10 – MQTTnet with C#

- [ ] Install MQTTnet
- [ ] Create MQTT Client
- [ ] Connect to Broker
- [ ] Subscribe to Sensor Topics
- [ ] Receive Messages

Resource: "MQTTnet Documentation" (https://github.com/dotnet/MQTTnet)

Day 11 – Background Services

- [ ] BackgroundService
- [ ] IHostedService
- [ ] Create MQTT Background Service
- [ ] Handle Reconnection and Errors

Resource: "ASP.NET Core Hosted Services" (https://learn.microsoft.com/en-us/aspnet/core/fundamentals/host/hosted-services)

Day 12 – Process & Store Sensor Data

- [ ] Receive Temperature, Humidity, and Ammonia
- [ ] Deserialize JSON
- [ ] Validate Sensor Readings
- [ ] Save Data using EF Core
- [ ] Handle Invalid Data

Day 13 – SignalR

- [ ] WebSockets Basics
- [ ] SignalR Hubs
- [ ] Create SignalR Hub
- [ ] Send Real-Time Sensor Updates

Resource: "SignalR Documentation" (https://learn.microsoft.com/en-us/aspnet/core/signalr/)

Day 14 – Practical Task

- [ ] Connect Backend to MQTT Broker
- [ ] Receive Data using MQTTnet
- [ ] Store Readings in SQL Server
- [ ] Send Updates using SignalR
- [ ] Test Complete Flow

---

Week 3 – Authentication, Alerts & Integration

Day 15 – Authentication & Authorization

- [ ] Authentication vs Authorization
- [ ] JWT
- [ ] Token Generation and Validation
- [ ] Roles and Policies
- [ ] Protect API Endpoints

Resources:

- "Authentication & Authorization Playlist" (https://youtube.com/playlist?list=PLOeFnOV9YBa4yaz-uIi5T4ZW3QQGHJQXi&si=pTCn45Zu_ITqqE6P)
- "ASP.NET Core Authentication" (https://learn.microsoft.com/en-us/aspnet/core/security/authentication/)
- "ASP.NET Core Authorization" (https://learn.microsoft.com/en-us/aspnet/core/security/authorization/)

Day 16 – Twilio SMS

- [ ] Twilio Setup
- [ ] Twilio Credentials
- [ ] Send SMS using C#
- [ ] Create Alert Service

Resource: "Twilio SMS with C#" (https://www.twilio.com/docs/messaging/quickstart/csharp-dotnet)

Day 17 – Alert Logic

- [ ] Define Sensor Thresholds
- [ ] Detect Abnormal Readings
- [ ] Save Alerts in Database
- [ ] Prevent Duplicate Alerts
- [ ] Trigger SMS Notifications

Day 18 – Security & Configuration

- [ ] Environment Variables
- [ ] Secure Credentials
- [ ] API Protection
- [ ] Input Validation
- [ ] Logging and Exception Handling

Resource: "ASP.NET Core Security" (https://learn.microsoft.com/en-us/aspnet/core/security/)

Day 19 – Testing

- [ ] Test APIs using Postman
- [ ] Test MQTT Reception
- [ ] Test Database Storage
- [ ] Test SignalR Updates
- [ ] Test SMS Alerts
- [ ] Test Invalid Sensor Data

Day 20 – Full System Integration

- [ ] Connect Raspberry Pi or Simulator
- [ ] Connect MQTT Broker
- [ ] Receive and Validate Sensor Data
- [ ] Store Data in SQL Server
- [ ] Update Dashboard using SignalR
- [ ] Send SMS Alerts using Twilio

Day 21 – Final Review

- [ ] Review Project Architecture
- [ ] Fix Bugs
- [ ] Test Complete System
- [ ] Organize Code and Services
- [ ] Complete Project README

---

Final Project Flow

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
        +----------> SignalR
        |               |
        |               v
        |           Dashboard
        |
        v
   Alert Service
        |
        v
     Twilio SMS
