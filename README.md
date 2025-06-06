# Recurring Task with Time-Based Notifications and Reminders

This Home Assistant automation blueprint sends recurring notifications at a set time and date, with reminders at a defined frequency if needed. It creates a task in a designated to-do list to track open tasks and allows marking tasks as done either via notification action or manually in the to-do list. The blueprint automatically schedules the next task or reminder date based on user interaction.

---

## Prerequisites

- Home Assistant is installed and running
- A to-do list integration is configured in Home Assistant
- [Home Assistant companion app](https://play.google.com/store/apps/details?id=io.homeassistant.companion.android) installed on your mobile device for actionable notifications

---

## Installation

Use the following badge to import the blueprint directly into your Home Assistant instance:

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2FItayGrinberg%2FHomeAssistant_RecurringTaskWithReminder%2Fblob%2Fmain%2FRecurringTaskWithReminder.yaml)

---

## Usage

1. Import the blueprint into your Home Assistant automation blueprints.
2. Create input helpers of type `input_datetime` for tracking the next notification and next reminder dates.
3. Configure the automation using the blueprint, specifying:
   - To-do list entity
   - Task name
   - First notification date
   - Task interval (days)
   - Reminder interval (days)
   - Wait time for user response (minutes, max 240)
   - Notification time
   - Notification title
   - Mobile device target for notifications
4. The automation will send notifications at the specified time if the date matches the first notification date, next notification date, or next reminder date.
5. The user can mark tasks as done via the notification action or manually in the to-do list.
6. The automation will schedule the next notification and reminders accordingly.

---

## Features

- Uses input_datetime helpers to track and control notification and reminder schedules
- Sends actionable notifications via the Home Assistant companion app
- Automatically adds and removes tasks in your to-do list
- Respects user interaction to adjust scheduling dynamically

---

## License

MIT License

---

Feel free to contribute or open issues for improvements and bug fixes!
