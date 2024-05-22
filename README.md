# Meet App

## Key Features:
- Filter Events by City
- Show/Hide Event Details
- Specify Number of Events
- Use the App When Offline
- Add an App Shortcut to the Home Screen
- Display Charts Visualizing Event Details



## Feature: Filter Events By City

  ### *Scenario: When user hasn’t searched for a city, show upcoming events from all cities.*
    Given the user has not searched for a city
    When the user views the events list
    Then the user sees upcoming events from all cities

  ### *Scenario: User should see a list of suggestions when they search for a city.*
    Given the user is on the search page
    When the user starts typing a city name
    Then the user sees a list of city suggestions

  ### *Scenario: User can select a city from the suggested list.*
    Given the user is typing a city name and sees suggestions
    When the user selects a city from the suggested list
    Then the user sees events filtered by the selected city



## Feature: Show/Hide Event Details

  ### *Scenario: An event element is collapsed by default.*
    Given the user is viewing the events list
    When the user sees an event element
    Then the event element is collapsed by default

  ### *Scenario: User can expand an event to see details.*
    Given the user is viewing a collapsed event element
    When the user clicks on the event element
    Then the event element expands to show details

  ### *Scenario: User can collapse an event to hide details.*
    Given the user is viewing an expanded event element
    When the user clicks on the event element again
    Then the event element collapses to hide details



## Feature: Specify Number of Events

  ### *Scenario: When user hasn’t specified a number, 32 events are shown by default.*
    Given the user has not specified the number of events to display
    When the user views the events list
    Then 32 events are shown by default

  ### *Scenario: User can change the number of events displayed.*
    Given the user is on the settings page
    When the user specifies a number of events to display
    Then the events list updates to show the specified number of events



## Feature: Use the App When Offline

  ### *Scenario: Show cached data when there’s no internet connection.*
    Given the user is offline
    When the user opens the app
    Then the app shows cached event data

  ### *Scenario: Show error when user changes search settings (city, number of events).*
    Given the user is offline
    When the user attempts to change search settings
    Then the app shows an error message



## Feature: Add an App Shortcut to the Home Screen

  ### *Scenario: User can install the meet app as a shortcut on their device home screen.*
    Given the user is on the app installation page
    When the user chooses to install the app
    Then the app is added as a shortcut on the device home screen



## Feature: Display Charts Visualizing Event Details

  ### *Scenario: Show a chart with the number of upcoming events in each city.*
    Given the user is on the events dashboard
    When the user views the event statistics
    Then a chart is displayed showing the number of upcoming events in each city
