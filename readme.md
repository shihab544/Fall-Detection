# Real Time fall Detection Using MATLAB And Phyphox Application

# PhyphoxGUIUpdated

## Overview

`PhyphoxGUIUpdated` is a MATLAB app designed to interface with a Phyphox sensor, allowing real-time data acquisition and visualization of acceleration data along the X, Y, and Z axes. The app features functionalities to start and stop data recording, save the acquired data, clear all plots, and detect falls based on the acceleration data.

## Features

- **IP Address Configuration**: Allows the user to specify the IP address of the Phyphox sensor.
- **Start and Stop Data Recording**: Starts and stops the acquisition of real-time acceleration data from the Phyphox sensor.
- **Save Data**: Saves the acquired data to the MATLAB workspace for further analysis.
- **Clear All**: Clears all plots and resets the fall detection status and count.
- **Real-Time Fall Detection**: Detects falls based on the acceleration data and provides visual and audio alerts.

## Components

- **Left Panel**: Contains buttons for starting, stopping, saving, and clearing data, as well as fields for configuring the IP address and displaying the fall status and count.
- **Right Panel**: Displays the acceleration data plots for the X, Y, and Z axes.

## Code Structure

### Properties

- **UI Components**: Definitions for the UI components like buttons, labels, panels, and axes.
- **Data Properties**: Variables for storing the IP address, control commands, web options, data arrays, and fall detection state.

### Methods

- **plotFunktion**: Placeholder for additional plotting logic.
- **findFallSegments**: Identifies fall segments based on the specified criteria.
- **pollData**: Continuously polls the Phyphox sensor for acceleration data, applies a moving average filter, detects falls, updates plots, and provides alerts.
- **Callback Functions**: Handles button presses and updates the UI components accordingly.
  - `startupFcn`: Initializes the app and plots.
  - `updateAppLayout`: Adjusts the app layout based on the window size.
  - `httpIP_AdressEditFieldValueChanged`: Updates the IP address based on user input.
  - `StartButtonPushed`: Starts data acquisition.
  - `StopButtonPushed`: Stops data acquisition.
  - `ClearAllButtonPushed`: Clears all plots and data.
  - `SaveButtonPushed`: Saves data to the MATLAB workspace.

### Component Initialization

- **createComponents**: Sets up the UI components and layouts for the app.

### App Creation and Deletion

- **App Constructor**: Creates and initializes the app.
- **App Deletion**: Cleans up the app upon deletion.

## Usage

1. **Set IP Address**: Enter the IP address of the Phyphox sensor in the designated field.
2. **Start Data Recording**: Click the 'Start' button to begin data acquisition.
3. **Monitor Fall Status**: Observe the fall status and count in the left panel.
4. **Stop Data Recording**: Click the 'Stop' button to halt data acquisition.
5. **Save Data**: Click the 'Save' button to export data to the MATLAB workspace.
6. **Clear Data**: Click the 'Clear All' button to reset plots and fall status.

## Dependencies

- **MATLAB**: The app is developed using MATLAB App Designer.
- **Phyphox App**: The app interfaces with the Phyphox sensor for data acquisition.

## Installation

1. Clone the repository.
2. Open `PhyphoxGUIUpdated.mlapp` in MATLAB App Designer.
3. Run the app from App Designer.
