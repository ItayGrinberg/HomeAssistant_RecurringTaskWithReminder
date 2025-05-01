# HomeAssistant_RecurringTaskWithReminder
This blueprint creates an automation that sends a recurring notification at a user-defined time and date. When triggered, a notification is sent to the selected user's phone. The notification includes an action to mark the task as done. If not marked as done, reminders are sent at the chosen interval until the task is done. For simplicity, the blueprint requires choosing a to-do list where it will store pending tasks until marked as done.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
    
## Prerequisites:

- The [Home Assistant companion app](https://play.google.com/store/apps/details?id=io.homeassistant.companion.android) must be installed.
- A designated to-do list must be created.

## Installation
1. Click the link below to import the blueprint:

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2FItayGrinberg%2FHomeAssistant_RecurringTaskWithReminder%2Fblob%2Fmain%2FRecurringTaskWithReminder.yaml)

## Usage

Once installed:
1. Create a to-do list where pending tasks will be stored. It only needs to be done once, as the list can be used for all tasks.
3. Create an automation using the blueprint.
4. Pick the created to-do list.
5. Enter the recurring task name.
6. Select the first notification date.
7. Select the interval at which that task is required, and the frequency of reminders until the task is completed.
8. Pick the time of the day you will be notified.
9. Enter the notification message.
11. Select the compatible device to be notified.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (\`git checkout -b feature/your-feature-name\`).
3. Make and commit your changes (\`git commit -am 'Add new feature'\`).
4. Push to the branch (\`git push origin feature/your-feature-name\`).
5. Create a new Pull Request.

For major changes, please open an issue first to discuss what you want to change.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
