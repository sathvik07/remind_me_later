# Remind-me-later API

A simple Django REST API for storing reminders with date, time, message, and delivery type (SMS or Email).

## Features

- Accepts reminders with `date`, `time`, `message`, and `reminder_type`
- Supports `reminder_type`: `sms` or `email`
- Stores data in SQLite (default, can be configured for PostgreSQL)
- Simple JSON API using Django REST Framework

## API Endpoint

**POST METHOD** `/api/reminders/create/`

### Request Body (JSON)

```json
{
  "date": "2025-05-11",
  "time": "14:00:00",
  "message": "Submit the assignment",
  "reminder_type": "email"
}

