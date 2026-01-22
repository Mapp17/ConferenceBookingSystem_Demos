# Conference Room Booking System — API Usage Examples

This document provides realistic, end-to-end usage examples for the Conference Room Booking System API.
It is intended for developers, reviewers, and testers to understand how the API behaves without reading backend code.

### All examples assume:

JSON request/response bodies

ISO 8601 UTC timestamps

Bearer token authentication

## Authentication

All protected endpoints require a bearer token in the Authorization header.

Header Format

Authorization: Bearer <access_token>


### Example:

Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...

## Room Management
Get All Rooms

Retrieve all conference rooms available in the system.

Request

GET /rooms
Authorization: Bearer <token>


Response — 200 OK

[
  {
    "id": "room-101",
    "name": "Conference Room A",
    "capacity": 10,
    "equipment": ["Projector", "Whiteboard"]
  },
  {
    "id": "room-102",
    "name": "Conference Room B",
    "capacity": 6,
    "equipment": ["TV Screen"]
  }
]

## Create a Room (Admin Only)

Request

POST /rooms
Authorization: Bearer <token>
Content-Type: application/json

{
  "name": "Conference Room C",
  "capacity": 12,
  "equipment": ["Projector", "Video Conferencing"]
}


Response — 201 Created

{
  "id": "room-103",
  "name": "Conference Room C",
  "capacity": 12,
  "equipment": ["Projector", "Video Conferencing"]
}

## Bookings
Create a Booking

Employees can book a room for a specific time slot.

Request

POST /bookings
Authorization: Bearer <token>
Content-Type: application/json

{
  "roomId": "room-101",
  "title": "Sprint Planning Meeting",
  "startTime": "2026-02-01T10:00:00Z",
  "endTime": "2026-02-01T11:00:00Z"
}


Response — 201 Created

{
  "id": "booking-555",
  "roomId": "room-101",
  "title": "Sprint Planning Meeting",
  "startTime": "2026-02-01T10:00:00Z",
  "endTime": "2026-02-01T11:00:00Z",
  "status": "Confirmed"
}

## Cancel a Booking

Request

DELETE /bookings/booking-555
Authorization: Bearer <token>


Response — 204 No Content

No response body

## Availability
Check Room Availability

Check which rooms are available for a given time window and capacity.

Request

GET /availability?startTime=2026-02-01T10:00:00Z&endTime=2026-02-01T11:00:00Z&capacity=8
Authorization: Bearer <token>


Response — 200 OK

[
  {
    "roomId": "room-102",
    "name": "Conference Room B",
    "capacity": 6
  },
  {
    "roomId": "room-103",
    "name": "Conference Room C",
    "capacity": 12
  }
]

## Error Handling
Booking Conflict

Returned when a room is already booked for the selected time period.

Response — 409 Conflict

{
  "error": {
    "code": "BOOKING_CONFLICT",
    "message": "The selected room is already booked during this time period."
  }
}
