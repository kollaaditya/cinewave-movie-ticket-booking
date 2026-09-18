# 🎬 CineWave – Movie Ticket Booking System

## Project Overview

CineWave is a movie ticket booking system designed using Pega Blueprint.

The system manages the complete movie ticket booking lifecycle from
request submission to booking confirmation and resolution.

## Application Details

- Application: Ticketing and Booking
- Case Type: Movie Ticket Request
- Business: CineWave Entertainment
- Platform: Pega Blueprint
- Location: India
- Language: English

## Case Lifecycle

Request Details
        ↓
Availability
        ↓
Approval
        ↓
Booking Execution
        ↓
Resolved

## Main Features

- Customer movie ticket request
- Movie and show selection
- Ticket count selection
- Seat selection
- Seat availability checking
- Seat reservation
- Ticket price calculation
- Total booking cost calculation
- UPI / Credit-Debit Card payment
- Booking confirmation or cancellation
- Cancellation reason validation
- E-ticket generation
- Booking status management
- Premium and Standard show routing
- SLA management

## Data Objects

### Movie
- Movie Name
- Genre

### Show
- Movie Name
- Show Date
- Show Time
- Seat Capacity
- Show Type

### Booking
- Customer
- Movie
- Show
- Number of Tickets
- Seat Numbers
- Ticket Price
- Total Booking Cost
- Payment Method
- Booking Status
- Ticket ID
- Execution Status

### Payment
- Payment ID
- Payment Method
- Amount
- Payment Status
- Transaction ID

## Personas

### Customer
Creates and manages movie ticket requests.

### Booking Agent
Checks availability and manages booking information.

### Ticketing Manager
Handles booking-related management activities.

### System
Performs automated processing and routing.

## Business Rules

### Seat Availability

Available Seats Count >= Number of Tickets

The booking can proceed only when sufficient seats are available.

### Total Booking Cost

Total Booking Cost = Ticket Price × Number of Tickets

### Show Routing

Premium → PremiumShowQueue

Standard → StandardShowQueue

### Booking Status

- Pending
- Confirmed
- Cancelled

Cancellation Reason is required when the booking is cancelled.

## SLA

- Goal: 1 day
- Deadline: 2 days
- Approaching-deadline handling is configured.

## Project Architecture

Customer
   ↓
Movie Ticket Request
   ↓
Request Details
   ↓
Availability
   ↓
Approval
   ↓
Booking Execution
   ↓
Booking / Payment
   ↓
Resolved

## Project Evidence

The `Screenshots` folder contains screenshots of the Pega Blueprint
configuration and preview/testing stages.

## Documentation

The complete project report is available in the `Documentation` folder.

## Demo

Demo Link:

PASTE YOUR PEGA DEMO/PREVIEW LINK HERE

## Author

Kolla Aditya

Artificial Intelligence & Data Science
