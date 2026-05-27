# Calendar API (Backend)

Backend service for a full-stack calendar management system built as a team project.

Originally developed as a final engineering project in collaboration with Google (Start@Google backend training program).

## Overview

This is a Spring Boot REST API that supports a multi-user calendar system with authentication, event management, sharing capabilities, and real-time updates.

The system follows a layered architecture using controllers, services, repositories, and domain entities.

## Core Features

### Authentication & Users

* Email-based registration and login
* GitHub OAuth authentication (separated auth service)
* Role-based access control (filters and permission layer)

### Calendar & Events

* Create, update, and delete events
* Public and private events
* Multi-user calendar sharing system
* Role-based event permissions

### Collaboration Model

* Event invitations with status tracking
* User roles within events (permission-controlled actions)
* Ability to join/leave shared events

### Real-time Features

* WebSocket-based updates for calendar changes
* Event notifications via socket triggers

### Notifications System

* Email and in-app notifications
* Event lifecycle notifications (invite, update, cancel, etc.)

### Time Zone Support

* User-specific time zone handling

## Architecture

* Spring Boot REST API
* Layered architecture:

  * Controllers (API layer)
  * Services (business logic)
  * Repositories (data access)
  * Entities (domain model)
* Modular authentication and GitHub login service
* Event-driven notification system using WebSockets

## Testing

The project includes unit and integration tests covering:

* authentication flows
* role permissions
* service layer logic
* event handling behavior

## Tech Stack

Java, Spring Boot, Hibernate, MySQL, WebSockets

Client repository: https://github.com/leonShapiro/calendar-client 
