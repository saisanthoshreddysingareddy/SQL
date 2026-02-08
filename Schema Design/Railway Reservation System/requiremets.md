 # Railway Reservation System - Requirements

1. The system shall maintain stations with station code, name, city, state, and geo-coordinates.
2. The system shall maintain trains with train number, name, operator, and service type (EXPRESS, SUPERFAST, LOCAL).
3. The system shall define routes as ordered station stops with arrival time, departure time, and day offset.
4. The system shall generate train runs for specific dates from a base timetable with calendar exceptions (ADDED, CANCELLED).
5. The system shall maintain coaches per train run with coach type (1A, 2A, 3A, SL, CC, 2S) and sequence order.
6. The system shall maintain seat/berth maps per coach type with positions, quotas, and layout metadata.
7. The system shall compute fares based on class, distance slabs, dynamic factors, and quota rules, and snapshot fares at booking time
8. Users shall create PNR bookings with origin station, destination station, travel date, class, and quota (GENERAL, TATKAL, LADIES, SR).
9. A booking shall contain one or more passengers with name, age, gender, berth preference, ID proof type, and concession details.
10. Booking statuses shall include INITIATED, CONFIRMED, RAC, WAITLISTED, and CANCELLED, with numeric tracking for RAC and WAITLIST.
11. The system shall allocate seats and berths for confirmed bookings and update RAC and WAITLIST queues atomically.
12. The system shall record payments with transaction ID, mode, status, and handle refunds with cancellation charges and time slabs.
13. The system shall allow boarding point changes and reflect updates in coach and seat allocation.
14. The system shall prepare charts at defined cut-off times and lock final allocations per train run and coach.
15. The system shall handle operational disruptions including cancellations and rescheduling with refunds or rebooking.
16. The system shall audit all state changes with timestamps and operator identifiers.
