class Appointment {
    - patient_name: str
    - doctor_name: str
    - date: str
    - time: str
    + get_details(): str
}

class AppointmentSystem {
    - appointments: dict
    - next_id: int
    + book_appointment(patient_name, doctor_name, date, time)
    + view_appointment(appointment_id)
}

AppointmentSystem --> Appointment : uses
