# Meet App

## Key Features:
- Filter Events by City
- Show/Hide Event Details
- Specify Number of Events
- Use the App When Offline
- Add an App Shortcut to the Home Screen
- Display Charts Visualizing Event Details

Feature: Filter Events By City
  Scenario: When user hasn’t searched for a city, show upcoming events from all cities.
  Scenario: User should see a list of suggestions when they search for a city.
  Scenario: User can select a city from the suggested list.

Feature: Show/Hide Event Details
  Scenario: An event element is collapsed by default.
  Scenario: User can expand an event to see details.
  Scenario: User can collapse an event to hide details.

Feature: Specify Number of Events
  Scenario: When user hasn’t specified a number, 32 events are shown by default.
  Scenario: User can change the number of events displayed.

Feature: Use the App When Offline
  Scenario: Show cached data when there’s no internet connection.
  Scenario: Show error when user changes search settings (city, number of events).

Feature: Add an App Shortcut to the Home Screen
  Scenario: User can install the meet app as a shortcut on their device home screen.

Feature: Display Charts Visualizing Event Details
  Scenario: Show a chart with the number of upcoming events in each city.
