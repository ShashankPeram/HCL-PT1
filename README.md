# HCL-PT1
import java.util.ArrayList;
import java.util.List;
import java.util.Scanner;

class Patient {
    private String name;
    private int age;
    private String gender;
    private String address;
    private String phoneNumber;

}

class Doctor {
    private String name;
    private String specialization;
    private String phoneNumber;

}

class Appointment {
    private Doctor doctor;
    private Patient patient;
    private String date;
    private String time;

}

public class HealthcareManagementSystem {
    private List<Patient> patients;
    private List<Doctor> doctors;
    private List<Appointment> appointments;

    public HealthcareManagementSystem() {
        patients = new ArrayList<>();
        doctors = new ArrayList<>();
        appointments = new ArrayList<>();
    }


    public static void main(String[] args) {
        HealthcareManagementSystem system = new HealthcareManagementSystem();
        Scanner scanner = new Scanner(System.in);

        while (true) {
            System.out.println("Welcome to the Healthcare Management System");
            System.out.println("1. Add Patient");
            System.out.println("2. Add Doctor");
            System.out.println("3. Schedule Appointment");
            System.out.println("4. View Appointments");
            System.out.println("5. Exit");
            System.out.print("Enter your choice: ");
            int choice = scanner.nextInt();

            switch (choice) {
                case 1:
                    // Add a new patient
                    break;
                case 2:
                    // Add a new doctor
                    break;
                case 3:
                    // Schedule an appointment
                    break;
                case 4:
                    // View appointments
                    break;
                case 5:
                    System.out.println("Exiting the system.");
                    System.exit(0);
                default:
                    System.out.println("Invalid choice. Please try again.");
            }
        }
    }
}
