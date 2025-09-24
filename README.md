# Elevate_task1

Entities & Relationships

Entities:

ParkingLot – Represents parking areas

ParkingSlot – Individual slots in a lot

Vehicle – Vehicles using the system

Booking – Parking bookings

Payment – Booking payments

Admin – Manages parking lots (optional)

Relationships:

ParkingLot has many ParkingSlots

Vehicle can have many Bookings

ParkingSlot can be booked multiple times

Booking has one Payment

Admin can manage multiple ParkingLots (optional)


Primary and Foreign Key

ParkingLot: PK = ParkingLotID – Attributes = Name, Location, TotalSlots, AvailableSlots

ParkingSlot: PK = SlotID – FK = ParkingLotID – Attributes = SlotNumber, SlotType, Status

Vehicle: PK = VehicleID – Attributes = OwnerName, VehicleNumber, VehicleType, ContactNumber

Booking: PK = BookingID – FK = VehicleID, SlotID – Attributes = StartTime, EndTime, Status, PaymentStatus

Payment: PK = PaymentID – FK = BookingID – Attributes = Amount, PaymentMode, PaymentDate

Admin (optional): PK = AdminID – FK = ParkingLotID – Attributes = Name, Email, Password


ER-Diagram

<img width="1920" height="835" alt="ER-Diagram" src="https://github.com/user-attachments/assets/a8e31a7f-6adc-4b17-903b-f3e036f686ec" />

