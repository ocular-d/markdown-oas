# Example

<!-- markdown-oas -->
 Endpoint                        | Method | Auth? | Description                                                                                                                                                             
 ------------------------------- | ------ | ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 `/stations`                     | GET    | No    | Returns a list of all train stations in the system.                                                                                                                     
 `/trips`                        | GET    | No    | Returns a list of available train trips between the specified origin and destination stations on the given date, and allows for filtering by bicycle and dog allowances.
 `/bookings`                     | GET    | No    | Returns a list of all trips booking by the authenticated user.                                                                                                          
 `/bookings`                     | POST   | Yes   | A booking is a temporary hold on a trip. It is not confirmed until the payment is processed.                                                                            
 `/bookings/{bookingId}`         | GET    | No    | Returns the details of a specific booking.                                                                                                                              
 `/bookings/{bookingId}`         | DELETE | Yes   | Deletes a booking, cancelling the hold on the trip.                                                                                                                     
 `/bookings/{bookingId}/payment` | POST   | No    | A payment is an attempt to pay for the booking, which will confirm the booking for the user and enable them to get their tickets.                                       
<!-- /markdown-oas -->
