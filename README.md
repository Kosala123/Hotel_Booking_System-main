## Hotel Booking System

## Description

- This system helps streamline hotel operations, including:
- Managing rooms
- Handling reservations
- Processing guest feedback
- Managing payments

## Key Entities

## 1. Room

The Room class models a hotel room, its attributes, and behaviours

Attributes:
room_id: Unique identifier for the room
location: Specifies the location or floor of the room
type: Indicates the type of room (e.g., "Single", "Double", "Suite")
price: Represents the price per night for the room
is_available: Boolean value to indicate the room’s availability status (default is True).

Methods:
check_availability(): Checks if the room is available for booking.
book_room(): Books the room and marks it as unavailable.
room_info(): Returns a string representation of the room’s details.
update_price(new_price): Updates the price of the room.
current_price(): Returns the current price of the room.

## 2. Admin

The Admin class represents hotel administrators with privileges for managing resources.

Attributes:
admin_id: Unique identifier for the admin.
name: Name of the admin.
contact_info: Contact details of the admin.
role: Role of the admin (e.g., "Manager").

Methods:
add_room(room): Adds a new room to the hotel.
remove_room(room_id): Removes a room from the hotel by its ID.
view_reservation(): Displays all reservations in the hotel.
manage_guest(guest): Manages guest information and reservations.
manage_employee(employee): Manages employee roles and assignments.

## 3. Guest

The Guest class models hotel guests and their information.

Attributes:
guest_id: Unique identifier for the guest.
name: Name of the guest.
contact_info: Contact details of the guest.

Methods:
contact_info(): Retrieves the guest’s contact information.
update_contact_info(new_contact): Updates the guest’s contact details.
guest_info(): Returns a string representation of the guest’s details.

## 4. Feedback

The Feedback class enables guests to submit feedback about their stay.

Attributes:
guest_id: ID of the guest submitting the feedback.
feedback_info: String containing the feedback details.

Methods:
submit_feedback(): Submits the feedback for the guest.
view_feedback(): Displays all feedback submitted by guests.

## 5. Reservation

The Reservation class handles bookings and maintains reservation details.

Attributes:
reservation_id: Unique identifier for the reservation.
guest_id: ID of the guest who made the reservation.
room_id: ID of the room booked.
check_in_date: Check-in date for the reservation.
check_out_date: Check-out date for the reservation.
is_active: Boolean indicating whether the reservation is active.

Methods:
confirm_reservation(): Confirms the reservation and marks the room as unavailable.
cancel_reservation(): Cancels the reservation and marks the room as available.
reservation_details(): Provides a string representation of the reservation details.
update_reservation_details(new_details): Updates the reservation details.

## 6. Payment

The Payment class manages payments and maintains a history of transactions.

Attributes:
reservation_id: ID of the reservation for which payment is made.
reservation_history: List of payment transactions for reservations.

Methods:
make_payment(amount): Processes payment for the specified amount.
view_payment_history(): Displays the payment history for all reservations.
calculate_total(): Calculates the total cost of a reservation based on the number of nights and room price.

## Contributors
1.Dileeshan Kosala
2.Aaaaaaaaaaa