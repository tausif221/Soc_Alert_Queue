# Initialize an empty list for the alert queue
alert_queue = []

# Main menu using while True loop
while True:
    print("\n--- SOC Active Alert Queue Menu ---")
    print("1. Log New Alert")
    print("2. View Active Queue")
    print("3. Resolve Oldest Alert")
    print("4. Exit System")

    choice = input("Enter your choice (1-4): ")

    if choice == "1":
        # Log New Alert
        threat_desc = input("Enter threat description: ")
        alert_queue.append(threat_desc)
        print("Alert logged successfully!")

    elif choice == "2":
        # View Active Queue
        print("--- Current Pending Alerts ---")

        if len(alert_queue) == 0:
            print("No active alerts in the queue.")
        else:
            for alert in alert_queue:
                print(f"- {alert}")

    elif choice == "3":
        # Resolve Oldest Alert
        if len(alert_queue) > 0:
            resolved_threat = alert_queue.pop(0)
            print(f"Resolved and cleared: {resolved_threat}")
        else:
            print("No pending alerts to resolve.")

    elif choice == "4":
        # Exit System
        print("Exiting SOC Alert Queue System.")
        break

    else:
        print("Invalid choice. Please enter a number between 1 and 4.")


