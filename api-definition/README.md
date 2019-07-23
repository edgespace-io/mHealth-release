# mHealth API Definition ![Release Status](https://img.shields.io/badge/Release-v0.1-green.svg)

## Create
Create a mHealth instance.

## Data Types

## Method Calls

### getSummaryData

| Param         | Type       | Description                                                               |
| ------------- | ---------- | ------------------------------------------------------------------------- |
| **Returns**   | `object`   | returns steps sleep, calories, and cura data for week/day/month for       |
| &nbsp;        | &nbsp;     | current date time to populate dashboard data                              |

### getStepsData

| Param         | Type       | Description                                                               |
| ------------- | ---------- | ------------------------------------------------------------------------- |
| **Returns**   | `step`     | returns sleep data for week/day/month for current date time               |

### getSleepData

| Param         | Type       | Description                                                               |
| ------------- | ---------- | ------------------------------------------------------------------------- |
| **Returns**   | `sleep`    | returns sleep data for week/day/month for current date time               |

### getCaloriesData

| Param         | Type       | Description                                                               |
| ------------- | ---------- | ------------------------------------------------------------------------- |
| **Returns**   | `calories` | returns calorie data for week/day/month for current date time             |

### getCuraData

| Param         | Type       | Description                                                               |
| ------------- | ---------- | ------------------------------------------------------------------------- |
| **Returns**   | `cura`     | returns cura data for standard 36 hour window based on current date time  |

### getDataRange

| Param         | Type       | Description                                                               |
| ------------- | ---------- | ------------------------------------------------------------------------- |
| dataType      | `String`   | Name of the [datatype](api#Data_Types) to retrieve.                       |
| startDate     | `date`     | Retrieve data from date, must be prior to current date time               |
| endDate       | `date`     | Retrieve data end date, must be less than or equal to current date time   |
| **Returns**   | `array`    | returns array of data type requested null if not found                    |

## Events

### dataUpdate

### alertNotification

