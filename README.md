# DayOfDusk_ReactorAPI
The ReactorAPI is for interfacing with the new reactor in Day of Dusk: The Border.

# ReactorLib Documentation

## Overview

ReactorLib is a Lua module designed for managing and monitoring a nuclear reactor simulation within a Roblox game. This library provides a suite of functions for fetching the reactor model, subscribing to reactor attribute changes, and getting current values of various reactor attributes such as fuel level, heat level, and power output.

## Functions

### FetchReactorModel

Fetches the reactor model (`FedoriumReactor`) from the workspace. If the model is not found, it throws a major error.

**Returns:**

- The `FedoriumReactor` model if found.

### SubscribeFuelChangeEvent

Returns an event that fires when the reactor's fuel level changes.

**Returns:**

- Fuel change event.

### SubscribeHeatChangeEvent

Returns an event that fires when the reactor's heat level changes.

**Returns:**

- Heat change event.

### SubscribeFuelUtilisationLevelChangeEvent

Returns an event that fires when the reactor's fuel utilization level changes.

**Returns:**

- Fuel utilization level change event.

### SubscribeFuelRodsInsertedChangeEvent

Returns an event that fires when the number of fuel rods inserted into the reactor changes.

**Returns:**

- Fuel rods inserted change event.

### SubscribePowerOutputChangeEvent

Returns an event that fires when the reactor's power output changes.

**Returns:**

- Power output change event.

### SubscribeActivityChangeEvent

Returns an event that fires when the reactor's activity status changes.

**Returns:**

- Activity change event.

### GetFuelLevel

Returns the current fuel level of the reactor.

**Returns:**

- Current fuel level.

### GetHeatLevel

Returns the current heat level of the reactor.

**Returns:**

- Current heat level.

### GetRodsInserted

Returns the current number of fuel rods inserted in the reactor.

**Returns:**

- Number of fuel rods inserted.

### GetFuelUtilisationLevel

Returns the current fuel utilization level of the reactor.

**Returns:**

- Current fuel utilization level.

### GetPowerOutput

Returns the current power output of the reactor.

**Returns:**

- Current power output.

### GetActiveValue

Returns the current activity status of the reactor.

**Returns:**

- Current activity status.

## Event Subscription

The library utilizes the `GetAttributeChangedSignal` method to subscribe to changes in reactor attributes. When an attribute changes, the corresponding event (e.g., `FuelChange`, `HeatChange`) is fired, allowing other scripts to react to these changes in real-time.

## Error Handling

If the `FedoriumReactor` model is not found in the workspace, the `FetchReactorModel` function will throw a major error, indicating a critical issue that must be resolved for the library to function correctly.

## Conclusion

`ReactorLib` provides a robust interface for managing a nuclear reactor within Roblox, offering real-time monitoring and event-driven management of reactor operations. This library is essential for developers looking to simulate nuclear reactor dynamics in their games.
